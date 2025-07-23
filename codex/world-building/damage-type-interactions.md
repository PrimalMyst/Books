# PrimalMyst Damage Type Interactions

## Hexagonal Interaction System

The six damage types form a hexagonal relationship where position determines interaction strength:

```
                    (1) COLD
                      /\
                     /  \
         (6) RADIANCE    (2) CHAOS
                   \    /
                    \  /
         (5) FIRE ---- ---- (3) LIGHTNING
                    \  /
                     \/
                (4) PHYSICAL
```

**Clockwise Order:** Cold → Chaos → Lightning → Physical → Fire → Radiance → Cold

## Interaction Rules

### Offensive Multipliers (Damage Dealt)
- **Next Type (+1):** 1.33x damage
- **Second Next (+2):** 1.66x damage  
- **Self (0):** 1.0x damage (neutral)
- **Opposite (+3):** 1.0x damage (neutral)
- **Second Previous (+4):** 0.66x damage
- **Previous (+5):** 0.33x damage

### Defensive Multipliers (Damage Taken)
- **Previous Type (-1):** 0.66x damage taken
- **Second Previous (-2):** 0.33x damage taken
- **Self (0):** 1.0x damage taken (neutral)
- **Opposite (-3):** 1.0x damage taken (neutral)
- **Second Next (-4):** 1.66x damage taken
- **Next (-5):** 1.33x damage taken

## Complete Interaction Table

| Attacker ↓ / Defender → | Cold | Chaos | Lightning | Physical | Fire | Radiance |
|-------------------------|------|-------|-----------|----------|------|----------|
| **Cold**               | 1.0x | 1.33x | 1.66x     | 1.0x     | 0.66x| 0.33x    |
| **Chaos**              | 0.33x| 1.0x  | 1.33x     | 1.66x    | 1.0x | 0.66x    |
| **Lightning**          | 0.66x| 0.33x | 1.0x      | 1.33x    | 1.66x| 1.0x     |
| **Physical**           | 1.0x | 0.66x | 0.33x     | 1.0x     | 1.33x| 1.66x    |
| **Fire**               | 1.66x| 1.0x  | 0.66x     | 0.33x    | 1.0x | 1.33x    |
| **Radiance**           | 1.33x| 1.66x | 1.0x      | 0.66x    | 0.33x| 1.0x     |

## Strategic Implications

### Offensive Strategy
- **Strong Against:** Next (+1) and Second Next (+2) types
- **Weak Against:** Previous (-1) and Second Previous (-2) types
- **Neutral:** Self and Opposite types

### Defensive Strategy  
- **Resistant To:** Previous (-1) and Second Previous (-2) types
- **Vulnerable To:** Next (+1) and Second Next (+2) types
- **Neutral:** Self and Opposite types

### Build Considerations

#### Pure Builds
- **Advantages:** Maximum effectiveness against specific targets
- **Disadvantages:** Clear vulnerabilities to specific damage types

#### Adjacent Builds (Hybrid)
- **Cold + Chaos:** Strong vs Lightning/Physical, weak vs Fire/Radiance
- **Chaos + Lightning:** Strong vs Physical/Fire, weak vs Radiance/Cold
- **Lightning + Physical:** Strong vs Fire/Radiance, weak vs Cold/Chaos
- **Physical + Fire:** Strong vs Radiance/Cold, weak vs Chaos/Lightning
- **Fire + Radiance:** Strong vs Cold/Chaos, weak vs Lightning/Physical
- **Radiance + Cold:** Strong vs Chaos/Lightning, weak vs Physical/Fire

#### Opposition Builds (Advanced)
- **Cold + Physical:** Complementary strengths and weaknesses
- **Chaos + Fire:** Balanced offensive/defensive profile
- **Lightning + Radiance:** High risk, high reward combinations

## Lore Justification

### The Cosmic Flow
The interaction pattern reflects the natural flow of cosmic energy through Yggdrasil's hexagonal structure:

- **Forward Flow (Stronger):** Energy flows naturally to the next positions in the cosmic cycle
- **Backward Resistance (Weaker):** Acting against the cosmic flow requires more effort
- **Neutral Points:** Self-interaction (pure mastery) and Opposition (perfect balance)

### Divine Relationships
- **Fundamental Gods** (Cold, Lightning, Fire) have complex interactions with **Primal Gods** (Chaos, Physical, Radiance)
- The pattern ensures no single divine influence dominates the cosmic balance
- Adjacent gods support each other's followers, while distant gods challenge them

## Gameplay Applications

### PvP Balance
- Rock-paper-scissors dynamics with multiple layers
- No single build dominates all situations
- Skill expression through damage type selection and timing

### PvE Design
- Enemy compositions can be designed around interaction weaknesses
- Players must consider damage type diversity in group composition
- Boss mechanics can emphasize different interaction patterns

### Equipment Design
- Conversion mechanics become strategically important
- Resistance gear provides meaningful choices
- Hybrid damage types offer tactical flexibility
