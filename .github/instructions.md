# PrimalMyst Canon Instructions

## Purpose
This file is the operating source of truth for documentation cleanup.
Use it to prevent non-canon concepts from spreading across the project.

## Canon Policy
- Stable foundation: colors, elements, positions, attributes, system relationships, mythological inspiration pairs.
- Mutable lore: god descriptions, tone, personality, realm flavor text, narrative examples.
- Rule: if foundation conflicts with lore, foundation always wins.

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

### League and Eternal Realm Model (locked)
- Leagues/seasons are real-world timeboxed cycles (ARPG seasonal model).
- Active season is where current story beats and live events happen.
- Myrielle and Valhalla/Eternal Realm exist permanently across all seasons.
- Valhalla/Eternal Realm long-term design exists but detailed implementation is intentionally undefined for now.

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
