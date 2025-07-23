# PrimalMyst Damage Calculator Reference

## Quick Reference Table

| Attacker ↓ / Defender → | Cold | Chaos | Lightning | Physical | Fire | Radiance |
|-------------------------|------|-------|-----------|----------|------|----------|
| **Cold**               | 1.0x | 1.33x | 1.66x     | 1.99x    | 0.34x| 0.67x    |
| **Chaos**              | 0.67x| 1.0x  | 1.33x     | 1.66x    | 1.99x| 0.34x    |
| **Lightning**          | 0.34x| 0.67x | 1.0x      | 1.33x    | 1.66x| 1.99x    |
| **Physical**           | 1.99x| 0.34x | 0.67x     | 1.0x     | 1.33x| 1.66x    |
| **Fire**               | 1.66x| 1.99x | 0.34x     | 0.67x    | 1.0x | 1.33x    |
| **Radiance**           | 1.33x| 1.66x | 1.99x     | 0.34x    | 0.67x| 1.0x     |

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

### Clockwise Order
1. Cold → 2. Chaos → 3. Lightning → 4. Physical → 5. Fire → 6. Radiance → 1. Cold

### TypeMult Pattern (0 → 1 → 2 → 3 → -2 → -1)
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
                PHYSICAL (3)
```

## Cross-Trio Warfare

### Fundamental vs Primal Opposition (1.99x effectiveness)
- **Cold → Physical:** Preservation shatters disciplined action with absolute stasis
- **Lightning → Radiance:** Raw connection overwhelms divine illumination with pure energy
- **Fire → Chaos:** Ordered transformation burns away chaotic corruption with focused heat

### Divine Warfare Philosophy
The **Fundamental Trio** and **Primal Trio** wage eternal war for cosmic supremacy. Each trio seeks to impose their vision of reality, making opposites the most bitter enemies who understand each other's weaknesses intimately.

## Calculation Examples

### Example 1: Cross-Trio Warfare (1.99x)
- **Cold attacking Physical:** typemult = 3 → 1 + 3 * 0.33 = 1.99x
- **Lightning attacking Radiance:** typemult = 3 → 1 + 3 * 0.33 = 1.99x
- **Fire attacking Chaos:** typemult = 3 → 1 + 3 * 0.33 = 1.99x

### Example 2: Intra-Trio Rivalry (1.66x)
- **Fire attacking Cold:** typemult = 2 → 1 + 2 * 0.33 = 1.66x
- **Chaos attacking Physical:** typemult = 2 → 1 + 2 * 0.33 = 1.66x
- **Lightning attacking Fire:** typemult = 2 → 1 + 2 * 0.33 = 1.66x

### Example 3: Adjacent Advantages (1.33x)
- **Cold attacking Chaos:** typemult = 1 → 1 + 1 * 0.33 = 1.33x
- **Lightning attacking Physical:** typemult = 1 → 1 + 1 * 0.33 = 1.33x
- **Fire attacking Radiance:** typemult = 1 → 1 + 1 * 0.33 = 1.33x

### Example 4: Self-Mastery (1.0x)
- **Any type vs Self:** typemult = 0 → 1 + 0 * 0.33 = 1.0x

### Example 5: Disadvantages
- **Strong (0.34x):** typemult = -2 → 1 + -2 * 0.33 = 0.34x
- **Moderate (0.67x):** typemult = -1 → 1 + -1 * 0.33 = 0.67x

## Implementation Notes

### Balance Considerations
- The 0.33 step creates distinct effectiveness tiers: 0.34x, 0.67x, 1.0x, 1.33x, 1.66x, 1.99x
- **Cross-trio warfare** (1.99x) creates the highest damage potential
- **Intra-trio rivalry** (1.66x) maintains strong within-trio competition
- Maximum advantage is 1.99x, minimum is 0.34x (nearly 6:1 ratio)
- System encourages diverse damage type usage and counter-play

### Strategic Meta
- **No neutral matchups:** Every damage type has clear strengths and weaknesses
- **Counter-picking emphasis:** Knowing enemy damage types becomes crucial
- **Build diversity required:** Pure builds become more risky but potentially more rewarding
- **Cross-trio opposition:** Fundamental vs Primal creates major strategic decisions

### Future Expansion
- Hybrid damage types can use weighted averages of base types
- Environmental modifiers can stack multiplicatively
- Status effects can temporarily modify typemult values
- Equipment can provide type resistance/vulnerability bonuses
