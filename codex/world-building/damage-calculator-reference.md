# PrimalMyst Damage Calculator Reference

## Quick Reference Table

| Attacker ↓ / Defender → | Cold | Chaos | Lightning | Physical | Fire | Radiance |
|-------------------------|------|-------|-----------|----------|------|----------|
| **Cold**               | 1.0x | 1.33x | 1.66x     | 1.0x     | 0.34x| 0.67x    |
| **Chaos**              | 0.67x| 1.0x  | 1.33x     | 1.66x    | 1.0x | 0.34x    |
| **Lightning**          | 0.34x| 0.67x | 1.0x      | 1.33x    | 1.66x| 1.0x     |
| **Physical**           | 1.0x | 0.34x | 0.67x     | 1.0x     | 1.33x| 1.66x    |
| **Fire**               | 1.66x| 1.0x  | 0.34x     | 0.67x    | 1.0x | 1.33x    |
| **Radiance**           | 1.33x| 1.66x | 1.0x      | 0.34x    | 0.67x| 1.0x     |

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
- **Opposite (+3):** typemult = 0 → 1 + 0 * 0.33 = **1.0x**
- **Second Previous (+4):** typemult = -2 → 1 + -2 * 0.33 = **0.34x**
- **Previous (+5):** typemult = -1 → 1 + -1 * 0.33 = **0.67x**

### Tuning Options
Adjusting `effectiveness_step` changes interaction strength:
- **0.25:** More subtle (1.0, 1.25, 1.5, 1.0, 0.5, 0.75)
- **0.33:** Current balanced (1.0, 1.33, 1.66, 1.0, 0.34, 0.67)
- **0.50:** More dramatic (1.0, 1.5, 2.0, 1.0, 0.0, 0.5)

## Hexagonal Position System

### Clockwise Order
1. Cold → 2. Chaos → 3. Lightning → 4. Physical → 5. Fire → 6. Radiance → 1. Cold

### TypeMult Pattern (0 → 1 → 2 → 0 → -2 → -1)
```
                    COLD (0)
                      /\
                     /  \
         RADIANCE (-1)   CHAOS (1)
                   \    /
                    \  /
         FIRE (-2) ---- ---- LIGHTNING (2)
                    \  /
                     \/
                PHYSICAL (0)
```

## Divine Trio Relationships

### Fundamental Trio (1.66x effectiveness)
- **Cold → Lightning:** Preservation grounds chaotic energy
- **Lightning → Fire:** Connection energizes heat into plasma  
- **Fire → Cold:** Transformation melts crystalline structures

### Primal Trio (1.66x effectiveness)
- **Chaos → Physical:** Creative disruption breaks discipline
- **Physical → Radiance:** Martial focus grounds ethereal power
- **Radiance → Chaos:** Divine light banishes shadow corruption

## Calculation Examples

### Example 1: Strong Advantages (1.66x)
- **Fire attacking Cold:** typemult = 2 → 1 + 2 * 0.33 = 1.66x
- **Chaos attacking Physical:** typemult = 2 → 1 + 2 * 0.33 = 1.66x
- **Lightning attacking Fire:** typemult = 2 → 1 + 2 * 0.33 = 1.66x

### Example 2: Moderate Advantages (1.33x)
- **Cold attacking Chaos:** typemult = 1 → 1 + 1 * 0.33 = 1.33x
- **Lightning attacking Physical:** typemult = 1 → 1 + 1 * 0.33 = 1.33x
- **Fire attacking Radiance:** typemult = 1 → 1 + 1 * 0.33 = 1.33x

### Example 3: Neutral (1.0x)
- **Any type vs Self:** typemult = 0 → 1 + 0 * 0.33 = 1.0x
- **Cold vs Physical:** typemult = 0 → 1 + 0 * 0.33 = 1.0x (opposites)
- **Chaos vs Fire:** typemult = 0 → 1 + 0 * 0.33 = 1.0x (opposites)

### Example 4: Disadvantages
- **Strong (0.34x):** typemult = -2 → 1 + -2 * 0.33 = 0.34x
- **Moderate (0.67x):** typemult = -1 → 1 + -1 * 0.33 = 0.67x

## Implementation Notes

### Balance Considerations
- The 0.33 step provides clear distinctions without extreme values
- Neutral matchups (1.0x) occur at self and opposite positions
- Maximum advantage is 1.66x, minimum is 0.34x
- System maintains mathematical symmetry

### Future Expansion
- Hybrid damage types can use weighted averages of base types
- Environmental modifiers can stack multiplicatively
- Status effects can temporarily modify typemult values
- Equipment can provide type resistance/vulnerability bonuses
