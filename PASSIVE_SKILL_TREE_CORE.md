# Passive Skill Tree — Core Spec (v0.1)

This document defines the core, system-level shape and rules for the Passive Skill Tree. It’s intentionally iterative so we can extend it with mechanics, visuals, and content later.

## Core requirements

- Points per level: 1 per level from 2 → 100 (total 99 points for levels 1–100).
- Tree layout: Hexagonal honeycomb of radius 6 (total cells = 127).
- Selection unit: Edges. Every hex cell has 6 edges; each edge is one selectable passive point.
- Cell activation: Selecting all 6 edges of a cell marks that cell Active.
- Perimeter rule: All outer perimeter edges of the big hexagon are always Active (do not cost points and cannot be unselected).
- Center rule: The central cell starts Active with all of its edges selected (do not cost points and cannot be unselected).
 - Connectivity rule: Players may only select edges that are connected to the central cell’s edges. Expansion proceeds outward; edges in cells not connected to the center are not selectable.
 - Adjacent-to-filled rule: A cell adjacent (edge-sharing) to a filled (Active) cell unlocks its edges for selection, allowing gradual completion of edge cells without requiring a new start point at the perimeter.
 - Perimeter connectivity: Perimeter edges are locked-active but do not provide connectivity for expansion (they cannot be used as starting points).

## Geometry

- Grid: Hex axial coordinates (q, r); cube s is implied by s = −q − r.
- Radius r = 6; total cells N = 1 + 3·r·(r+1) = 127.
- Unique edges: E = (6·N + 6·r)/2 = 399. Of these, perimeter edges = 6·r = 36.

We’ll store the tree procedurally with radius + rules. Explicit cells/edges can be added later if needed (for authored clusters, art alignment, or special routing).

### Radius variants (for comparison)

We treat radius as a variable so we can compare alternatives:

- r = 5 → total cells N = 91 → min active cells = 1 (center only) → max active cells = 91
- r = 6 → total cells N = 127 → min active cells = 1 → max active cells = 127
- r = 7 → total cells N = 169 → min active cells = 1 → max active cells = 169

Notes:
- Perimeter edges are locked-active but don’t automatically fully activate perimeter cells.
- Max active cells assumes all selectable edges are taken under the rules (center-seeded connectivity, no perimeter starts).

### Activation bounds with 99 allocable edges

Let S = 99 allocable edges. Each selected edge contributes to 2 cells (shared edge), so total credit from selections is 2S = 198. A cell activates at 6 credits (edges). Freebies: center’s 6 edges (already active) give 1 free credit to each of its 6 neighbors; perimeter contributes 6r free credits (one per perimeter cell). Upper bound for newly activated cells M (excluding center) satisfies:

- If M ≤ (6 + 6r): 2S + M ≥ 6M ⇒ M ≤ floor(2S/5) = 39.
- If M > (6 + 6r): 2S + (6 + 6r) ≥ 6M ⇒ M ≤ floor((2S + 6 + 6r)/6).

Results (including the center cell):
- r = 5 (N=91): min = 1; max upper bound = 1 + 39 = 40
- r = 6 (N=127): min = 1; max upper bound = 1 + 39 = 40
- r = 7 (N=169): min = 1; max upper bound = 1 + 39 = 40

Note: 40 is a budget-limited upper bound assuming perfect sharing and fully leveraging one freebie per completed cell when possible. Actual achievable maxima will depend on layout routing; connectivity from center is compatible with approaching this bound using compact clusters.

## Progression contract

- Input: character level L in [1, 100].
- Output: total allocable passive points = max(0, min(L, 100) − 1).
- Notes: Perimeter edges and central cell edges are granted by system rules and do not consume points.

## Next iterations

- Named passive clusters and notables mapped to edge sets.
- Attribute scaling, synergies, and keystones that require patterns (rings, spokes, etc.).
- Character save schema for allocations and validation.

## Selection flow (summary)

1) Start state: Center cell’s 6 edges are locked active and count as the connectivity origin.
2) Expansion: You can allocate an edge if it belongs to a cell that is connected via cells/edges to the center OR the cell is adjacent to any Active (filled) cell.
3) Perimeter: Perimeter edges remain locked-active but do not serve as connectivity seeds; reaching outer cells still requires a connected path from the center.
