# PrimalMyst Canon Instructions

## Purpose
This file is the operating source of truth for documentation cleanup.
Use it to prevent non-canon concepts from spreading across the project.

## Canon Policy
- Stable foundation: colors, elements, positions, attributes, system relationships, mythological inspiration pairs.
- Mutable lore: god descriptions, tone, personality, realm flavor text, narrative examples.
- Rule: if foundation conflicts with lore, foundation always wins.

## Terminology Standard (locked)
- Use "diegetic framing" as the umbrella term for explaining game systems through in-world fiction.
- Use "diegetic UI" only for UI-specific in-world presentation (HUD, menus, indicators).
- Treat immersion as an outcome, not a replacement term for diegetic framing.
- Use "season" as the standard term for the timeboxed ARPG cycle.
- Use "character" as the standard term for player-controlled avatars in mechanics and general documentation.
- Reserve "league" and "vessel" for legacy references or diegetic-framing context only when needed.

## Codex Hierarchy and Ownership (locked)
- canon-core: immutable canon mappings, non-negotiable system truths, and rule authority.
- mechanics: gameplay rules, formulas, triggers, constraints, and edge cases.
- diegetic-framing: in-world fiction that explains how mechanics manifest in the setting.
- entities: gods, factions, races, monster families, and actor-focused references.
- lore: stable world context, cosmology, cultures, and setting truths outside timeline sequencing.
- story: timeline progression, acts, arcs, quests, and event sequencing.
- indexes: navigation files only (tables of contents, link maps, relationship indexes).

## Overlap Minimization Rules (required)
1. One concept has one primary owner layer.
2. Other layers may reference the concept, but must not redefine the owner's source of truth.
3. Mechanics files must not contain balancing-by-prose lore explanations.
4. Diegetic-framing files must not contain formulas, numeric tuning, or implementation constraints.
5. Story files describe when events happen, not canon remapping.
6. Index files link and summarize only; they never introduce new canon.

## Cross-Layer Pairing Pattern (required)
- For any gameplay concept with narrative framing, keep a paired set:
	- mechanics file: explains system behavior.
	- diegetic-framing file: explains in-world meaning.
- Example: world reset requires one mechanics document and one diegetic-framing document.

## Reference Preservation Standard (required)
- Use a shared Concept ID across all related files, format: CONCEPT-<TOPIC>-<NAME>.
- Each related file should include:
	- Concept ID
	- Owner Layer
	- Related Files
	- Status (draft or locked)
- Always keep explicit markdown links between paired mechanics and diegetic-framing files.

## Locked Core Concepts

### Hex Position System (locked)
- Position 1: Top/North
- Numbering direction: clockwise
- Positions are corners (not edges or faces)

### Core Mapping (locked)
1. Position 1 | Red | Fire | Strength | Primal | Ifrisurtr | Ifrit + Surtr
2. Position 2 | Yellow | Metal | Constitution | Sovereign | Longares | Dragon + Ares
3. Position 3 | Green | Air | Dexterity | Primal | Kitsunrir | Fenrir + Kitsune
4. Position 4 | Cyan | Lightning | Wisdom | Sovereign | Gryphozeus | Zeus + Griffin
5. Position 5 | Blue | Water | Intelligence | Primal | Tiamangandr | Tiamat + Jormungandr
6. Position 6 | Magenta | Shadow | Charisma | Sovereign | Bastenyx | Bastet + Nyx

### Tier Pattern (locked)
- Primal positions: 1, 3, 5 (RGB anchors)
- Sovereign positions: 2, 4, 6 (bridge colors)

### Resource/Defense Pattern (locked)
- Primal: Health Points, Stamina Points, Mana Points
- Sovereign: Armor, Energy Shield, Evasion

### Hidden Seventh (locked)
- Myrielle is outside the six-corner system.
- Myrielle is never assigned to positions 1-6.

### Season and Realm Model (locked)
- Seasons are real-world timeboxed cycles (ARPG seasonal model).
- The current season is partitioned by two difficulty flags, creating four concurrent realities:
	- default
	- hardcore
	- solo self found
	- hardcore solo self found
- Hardcore flag: characters that die are permanently lost.
- Solo self found flag: players cannot trade with other players.
- The current season is where current story beats and live events happen.
- The permanent realm is Valhalla and contains characters that successfully migrated from previous seasons.
- Myrielle and Valhalla exist permanently across all seasons.

## Deprecated and Forbidden Legacy Terms
Do not reintroduce these names in canon files:
- Pyrion, Glacius, Voltharion
- Serafina, Aurelius, Korthak
- Aquarix, Verdania, Umbros, Luxara, Zephyros

Do not reintroduce old damage sets as canon:
- Fire, Cold, Lightning, Holy, Chaos, Physical
- Fire, Physical, Lightning, Radiance, Cold, Chaos

## Editing Rules for Remaining Cleanup
1. Preserve locked core concepts exactly.
2. Rewrite conflicting lore to fit the locked core.
3. Keep storytelling flexible and clearly lore-scoped.
4. Prefer consistent terms: Primal (1/3/5), Sovereign (2/4/6).
5. If a file is uncertain, mark statement as lore (subject to change) instead of changing core.

## Step-by-Step Cleanup Process
1. Scan target file for forbidden legacy names and old damage sets.
2. Scan for old tier framing (Fundamental vs Primal) and update to Primal vs Sovereign.
3. Verify positional mappings against the locked core mapping.
4. Verify resource/defense assignments by tier.
5. Keep or rewrite prose as lore, but never alter locked mapping.
6. Run a final legacy-name grep over edited scope.

## Validation Checklist (required before closing each file)
- No forbidden legacy names remain.
- No old damage set is used as canon.
- Position, color, element, attribute, and tier match locked mapping.
- Myrielle remains outside positions 1-6.
- Any speculative description is framed as lore.

## Priority Cleanup Order
1. Root README and world-building overview files
2. Core system files (damage, hex, progression, race frameworks)
3. Lore act files and narrative examples
4. Supporting indexes and summaries

## Final Authority
If any document disagrees with this file, this file is correct.
