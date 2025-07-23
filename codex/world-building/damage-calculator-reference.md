# PrimalMyst Damage Calculator Reference

## Quick Reference Table

| Attacker ↓ / Defender → | Cold | Chaos | Lightning | Physical | Fire | Radiance |
|-------------------------|------|-------|-----------|----------|------|----------|
| **Cold**               | 1.0x | 1.33x | 1.66x     | 1.0x     | 0.66x| 0.33x    |
| **Chaos**              | 0.33x| 1.0x  | 1.33x     | 1.66x    | 1.0x | 0.66x    |
| **Lightning**          | 0.66x| 0.33x | 1.0x      | 1.33x    | 1.66x| 1.0x     |
| **Physical**           | 1.0x | 0.66x | 0.33x     | 1.0x     | 1.33x| 1.66x    |
| **Fire**               | 1.66x| 1.0x  | 0.66x     | 0.33x    | 1.0x | 1.33x    |
| **Radiance**           | 1.33x| 1.66x | 1.0x      | 0.66x    | 0.33x| 1.0x     |

## Calculation Examples

### Example 1: Cold vs Lightning
- **Cold attacking Lightning:** 1.66x damage (strong)
- **Lightning attacking Cold:** 0.66x damage (weak)
- **Relationship:** Cold (+2 position) vs Lightning, Lightning (-2 position) vs Cold

### Example 2: Physical vs Chaos  
- **Physical attacking Chaos:** 0.66x damage (weak)
- **Chaos attacking Physical:** 1.66x damage (strong)
- **Relationship:** Physical (-1 position) vs Chaos, Chaos (+2 position) vs Physical

### Example 3: Fire vs Radiance
- **Fire attacking Radiance:** 1.33x damage (moderate strong)
- **Radiance attacking Fire:** 0.33x damage (weak)
- **Relationship:** Fire (+1 position) vs Radiance, Radiance (-1 position) vs Fire

## Position Relationships

### Clockwise Order
1. Cold → 2. Chaos → 3. Lightning → 4. Physical → 5. Fire → 6. Radiance → 1. Cold

### Relationship Types
- **Self (0):** 1.0x - Perfect mastery, no advantage
- **Next (+1):** 1.33x offensive / 1.33x defensive vulnerability  
- **Second Next (+2):** 1.66x offensive / 1.66x defensive vulnerability
- **Opposite (+3):** 1.0x - Balanced opposition, no advantage
- **Second Previous (+4):** 0.66x offensive / 0.66x defensive resistance
- **Previous (+5):** 0.33x offensive / 0.33x defensive resistance

## Strategic Applications

### Build Planning
- **Pure Builds:** Maximize one damage type, accept clear weaknesses
- **Adjacent Builds:** Combine neighboring types for synergy (e.g., Cold+Chaos)
- **Opposition Builds:** Combine opposite types for balance (e.g., Cold+Physical)

### Combat Tactics
- **Target Selection:** Prioritize enemies weak to your damage type
- **Defensive Positioning:** Avoid enemies using your weakness types
- **Elemental Conversion:** Use gear/skills to convert damage to advantageous types

### Equipment Considerations
- **Resistance Gear:** Focus on protecting against your primary weaknesses
- **Conversion Effects:** Items that change incoming damage types
- **Hybrid Scaling:** Equipment that benefits from multiple damage types

## Implementation Notes

### Game Balance
- No damage type is universally superior
- Each type has exactly 2 advantages and 2 disadvantages
- Neutral relationships prevent hard counters
- Encourages diverse team compositions

### PvP Applications
- Creates natural rock-paper-scissors dynamics
- Skill expression through damage type selection
- Rewards adaptation and counter-play
- Prevents single-build dominance

### PvE Design
- Enemy types can be designed around interaction patterns
- Boss phases can shift damage type focus
- Group content rewards diverse damage types
- Resistance/immunity mechanics gain strategic depth
