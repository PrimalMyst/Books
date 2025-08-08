# PrimalMyst Damage Calculator Reference

## System Overview

This damage effectiveness system is based on the **Core Thematic Hexagon** (`data/json/lore/core-thematic-hexagon.json`) and implements the generic formulas defined in **Damage System Core** (`data/json/damage-types/damage-system-core.json`).

The system reflects the cosmic structure of Yggdrasil and the divine relationships between the Eldritch Pantheon, where damage effectiveness is determined by hexagonal positioning and divine opposition patterns.

## Quick Reference Table

| Attacker ↓ / Defender → | Fire | Physical | Lightning | Radiance | Cold | Chaos |
|-------------------------|------|----------|-----------|----------|------|-------|
| **Fire**               | 1.0x | 1.33x    | 1.66x     | 1.99x    | 0.34x| 0.67x |
| **Physical**           | 0.67x| 1.0x     | 1.33x     | 1.66x    | 1.99x| 0.34x |
| **Lightning**          | 0.34x| 0.67x    | 1.0x      | 1.33x    | 1.66x| 1.99x |
| **Radiance**           | 1.99x| 0.34x    | 0.67x     | 1.0x     | 1.33x| 1.66x |
| **Cold**               | 1.66x| 1.99x    | 0.34x     | 0.67x    | 1.0x | 1.33x |
| **Chaos**              | 1.33x| 1.66x    | 1.99x     | 0.34x    | 0.67x| 1.0x  |

## Calculation System

### Formula
```
damagetype_mult = 1 + typemult * effectiveness_step
```

### Parameters
- **effectiveness_step:** 0.33

### TypeMult Sequence (hexagonal position)
- **Self (0):** typemult = 0 → 1 + 0 * 0.33 = **1.0x**
- **Next (+1):** typemult = 1 → 1 + 1 * 0.33 = **1.33x**
- **Second Next (+2):** typemult = 2 → 1 + 2 * 0.33 = **1.66x**
- **Opposite (+3):** typemult = 3 → 1 + 3 * 0.33 = **1.99x**
- **Second Previous (+4):** typemult = -2 → 1 + -2 * 0.33 = **0.34x**
- **Previous (+5):** typemult = -1 → 1 + -1 * 0.33 = **0.67x**

### Tuning Options
Adjusting `effectiveness_step` changes interaction strength:
- **0.25:** More subtle (1.0, 1.25, 1.5, 1.75, 0.5, 0.75)
- **0.33:** Current balanced (1.0, 1.33, 1.66, 1.99, 0.34, 0.67)
- **0.50:** More dramatic (1.0, 1.5, 2.0, 2.5, 0.0, 0.5)

## Hexagonal Position System

### Positioning Reference (from core-thematic-hexagon.json)
1. **Fire** (Pyrion, the First Flame) - Red - Primal Anchor
2. **Physical** (Korthak, the Dragon King) - Yellow - Sovereign Bridge  
3. **Lightning** (Voltharion, the Cosmic Spark) - Green - Primal Anchor
4. **Radiance** (Aurelius, the Radiant Sphere) - Cyan - Sovereign Bridge
5. **Cold** (Glacius, the Eternal Frost) - Blue - Primal Anchor
6. **Chaos** (Serafina, the Shadow Empress) - Magenta - Sovereign Bridge

### Clockwise Order
1. Fire → 2. Physical → 3. Lightning → 4. Radiance → 5. Cold → 6. Chaos → 1. Fire

### TypeMult Pattern (0 → 1 → 2 → 3 → -2 → -1)
```
                    FIRE (0) 🔴
                      /\
                     /  \
         CHAOS (-1) 💜   PHYSICAL (1) 💛
                   \    /
                    \  /
         COLD (-2) 🔵 ---- ---- LIGHTNING (2) 🟢
                    \  /
                     \/
                RADIANCE (3) 🌊
```

## RGB Anchor vs Bridge Opposition

### RGB Anchors vs Sovereign Bridges (Opposite effectiveness)
- **Fire → Radiance:** Primal creation overwhelms divine order with raw transformative energy
- **Lightning → Chaos:** Primal connection grounds chaotic unpredictability with precise electrical patterns  
- **Cold → Physical:** Primal preservation freezes disciplined action with absolute crystalline stasis

### Divine Warfare Philosophy
The **RGB Anchor Gods** (Primal) and **Bridge Gods** (Sovereign) represent different approaches to cosmic power. RGB anchors provide foundational forces, while bridges create transitions and balance. Opposites create the most dramatic conflicts where pure elemental force meets refined divine technique.

## Calculation Examples

### Example 1: RGB vs Bridge Opposition (1.99x)
- **Fire attacking Radiance:** typemult = 3 → 1 + 3 * 0.33 = 1.99x
- **Lightning attacking Chaos:** typemult = 3 → 1 + 3 * 0.33 = 1.99x  
- **Cold attacking Physical:** typemult = 3 → 1 + 3 * 0.33 = 1.99x

### Example 2: Strong Advantages (1.66x)
- **Fire attacking Lightning:** typemult = 2 → 1 + 2 * 0.33 = 1.66x
- **Physical attacking Radiance:** typemult = 2 → 1 + 2 * 0.33 = 1.66x
- **Lightning attacking Cold:** typemult = 2 → 1 + 2 * 0.33 = 1.66x

### Example 3: Adjacent Advantages (1.33x)
- **Fire attacking Physical:** typemult = 1 → 1 + 1 * 0.33 = 1.33x
- **Lightning attacking Radiance:** typemult = 1 → 1 + 1 * 0.33 = 1.33x
- **Cold attacking Chaos:** typemult = 1 → 1 + 1 * 0.33 = 1.33x

### Example 4: Self-Mastery (1.0x)
- **Any type vs Self:** typemult = 0 → 1 + 0 * 0.33 = 1.0x

### Example 5: Disadvantages
- **Strong (0.34x):** typemult = -2 → 1 + -2 * 0.33 = 0.34x
- **Moderate (0.67x):** typemult = -1 → 1 + -1 * 0.33 = 0.67x

## Implementation Notes

### Balance Considerations
- The 0.33 step creates distinct effectiveness tiers: 0.34x, 0.67x, 1.0x, 1.33x, 1.66x, 1.99x
- **RGB vs Bridge opposition** (1.99x) creates the highest damage potential
- **Skip-one positioning** (1.66x) maintains strong tactical advantages
- Maximum advantage is 1.99x, minimum is 0.34x (nearly 6:1 ratio)
- System encourages diverse damage type usage and counter-play

### Strategic Meta
- **No neutral matchups:** Every damage type has clear strengths and weaknesses
- **Counter-picking emphasis:** Knowing enemy damage types becomes crucial
- **Build diversity required:** Pure builds become more risky but potentially more rewarding
- **RGB vs Bridge tension:** Primal anchors vs Sovereign bridges creates major strategic decisions

### Future Expansion
- Hybrid damage types can use weighted averages of base types
- Environmental modifiers can stack multiplicatively
- Status effects can temporarily modify typemult values
- Equipment can provide type resistance/vulnerability bonuses

## Related Files and Systems

### Core System Files
- **Core Thematic Hexagon**: `data/json/lore/core-thematic-hexagon.json`
- **Damage System Core**: `data/json/damage-types/damage-system-core.json`

### Individual Damage Types
- **Fire**: `data/json/damage-types/fire-damage.json`
- **Physical**: `data/json/damage-types/physical-damage.json`
- **Lightning**: `data/json/damage-types/lightning-damage.json`
- **Radiance**: `data/json/damage-types/radiance-damage.json`
- **Cold**: `data/json/damage-types/cold-damage.json`
- **Chaos**: `data/json/damage-types/chaos-damage.json`

### Lore and World-Building
- **Eldritch Pantheon**: `codex/lore/eldritch-pantheon.md`
- **Six Realms Cosmology**: `codex/lore/six-realms-cosmology.md`
- **Yggdrasil Lore**: `codex/lore/yggdrasil.md`

## Implementation Notes

All damage calculations should reference the **damage-system-core.json** for consistency and use the positioning data from **core-thematic-hexagon.json** as the authoritative source for hexagonal relationships.
