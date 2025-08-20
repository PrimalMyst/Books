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

Let S = 99 allocable edges. Each selected edge provides 2 “credits” (one to each incident cell). A cell activates at 6 credits. Free edges (“freebies”):
- Center-to-ring1: +6 total credits (1 to each of the 6 neighbors of center).
- Perimeter: +3 credits to each perimeter cell you activate (its 3 outer edges are free).

Maximize newly activated cells m (excluding the center) subject to credit conservation:
- 6m ≤ 2S + 6 + 3P, where P is the count of activated perimeter cells (P ≤ min(m, 6r)).
- For r ∈ {5,6,7}, the optimum is m > 6r, so set P = 6r. Then 6m ≤ 2S + 6 + 18r ⇒ m = (2S + 6 + 18r)/6 = 34 + 3r.

Totals including the center (T = m + 1):
- r = 5 (N = 91): m = 49 ⇒ T = 50
- r = 6 (N = 127): m = 52 ⇒ T = 53
- r = 7 (N = 169): m = 55 ⇒ T = 56

These values are tight by the credit model (equalities hold), and are compatible with center-seeded connectivity once you route to the perimeter.

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
