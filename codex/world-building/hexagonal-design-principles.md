# Hexagonal Design Principles

## Core Philosophy

PrimalMyst uses a **hexagonal preference** as its fundamental design pattern. This six-sided structure creates natural balance, meaningful relationships, and intuitive gameplay patterns throughout all systems.

## Design Pattern Structure

### Core Hexagon Architecture
- **Central Core**: The main organizing concept (like Yggdrasil for damage types)
- **Six Corners**: Individual elements arranged in meaningful sequence
- **Adjacency Relationships**: Natural synergies between neighboring elements
- **Opposition Dynamics**: Meaningful tension between opposite elements
- **Index System**: Each corner numbered 1-6 for consistent reference

### Implementation Standards

#### File Organization
```
data/json/{hexagon-type}/
├── {hexagon-type}-core.json          # Core hexagon with indexes
└── corners/
    ├── corner-1-{name}.json          # Individual corner details
    ├── corner-2-{name}.json
    ├── corner-3-{name}.json
    ├── corner-4-{name}.json
    ├── corner-5-{name}.json
    └── corner-6-{name}.json
```

#### Reference Pattern
- **Core files** contain the central concept and corner indexes
- **Corner files** contain detailed implementation for each position
- **Cross-references** link to related hexagon systems
- **Schemas** ensure consistent structure across all hexagons

## Active Hexagonal Systems

### 1. Eldritch Gods (Existing - References Only)
- **Core**: Eldritch Pantheon structure
- **Pattern**: Fundamental/Primal alternating trios
- **Location**: `eldritch-pantheon.json`
- **Status**: Established, no changes needed

### 2. Damage Types (Existing - References Only)  
- **Core**: Yggdrasil and elemental balance
- **Pattern**: Elemental progression around six corners
- **Location**: `damage-types/` directory
- **Status**: Established, no changes needed

### 3. Offensive Layers (New Implementation)
- **Core**: Combat attack methodologies
- **Pattern**: Attack styles and damage delivery systems
- **Location**: `offensive-layers/` directory
- **Status**: To be implemented

### 4. Defensive Layers (New Implementation)
- **Core**: Protection and mitigation strategies
- **Pattern**: Defense types and survival mechanisms  
- **Location**: `defensive-layers/` directory
- **Status**: To be implemented

### 5. Attributes (New Implementation)
- **Core**: Character development and growth
- **Pattern**: Core statistics and secondary attributes
- **Location**: `attributes/` directory
- **Status**: To be implemented

## Hexagonal Interaction Principles

### Adjacency Bonuses
- Elements next to each other provide natural synergies
- Combination builds gain effectiveness bonuses
- Transition paths feel intuitive and smooth

### Opposition Dynamics
- Opposite corners create meaningful choice tension
- Not absolute incompatibility, but requires investment
- Provides strategic depth and build diversity

### Full Spectrum Mastery
- Characters using all six corners gain special abilities
- Represents ultimate understanding of the system
- Extremely challenging but uniquely rewarding

## Cross-Hexagon Integration

### Overlay Mapping
Different hexagonal systems overlay meaningfully:
- Position 1 in all hexagons share thematic resonance
- Same adjacency patterns create consistent synergies
- Opposition patterns remain consistent across systems

### Design Consistency
- Same numbering system (1-6, clockwise from top)
- Similar relationship patterns between systems
- Unified thematic progression around the circle

## Implementation Guidelines

### New Hexagon Creation
1. **Identify the central organizing concept**
2. **Arrange six elements in meaningful sequence**
3. **Establish adjacency synergies**
4. **Define opposition tensions**
5. **Create core index file with references**
6. **Implement detailed corner files**
7. **Integrate with existing hexagonal systems**

### Schema Compliance
- Use `hexagon-thematic.schema.json` as base
- Extend with system-specific properties
- Maintain consistent relationship structures
- Include cross-references to other hexagons

### Documentation Standards
- Clear explanation of central concept
- Detailed corner descriptions
- Relationship mechanics explanation
- Integration with other systems
- Lore and mechanical justification

## Benefits of Hexagonal Design

### For Players
- **Intuitive Learning**: Consistent patterns across all systems
- **Strategic Depth**: Multiple viable paths and combinations
- **Progressive Mastery**: Natural advancement from simple to complex
- **Meaningful Choices**: Clear trade-offs and synergies

### For Developers
- **Systematic Design**: Consistent framework for all systems
- **Balanced Complexity**: Six elements provide richness without overwhelming
- **Cross-System Integration**: Natural ways to combine different mechanics
- **Scalable Architecture**: Pattern extends to new systems easily

### For World-Building
- **Thematic Consistency**: All systems reflect same cosmic structure
- **Lore Integration**: Mechanical systems reinforce narrative elements
- **Cosmic Logic**: Game rules reflect the universe's fundamental nature
- **Mystical Resonance**: Players feel connected to the world's deeper truths

---

*The hexagonal preference ensures that PrimalMyst's complexity serves clarity rather than confusion, creating a universe where understanding the pattern unlocks both mechanical mastery and cosmic wisdom.*
