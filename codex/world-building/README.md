# World Building Guide

## Overview

This directory contains comprehensive world-building documentation for PrimalMyst. All content here should align with the structured JSON data in the `/data` folder and serve as the narrative foundation for the game world.

## Directory Structure

```
world-building/
├── README.md                    # This file
├── cosmology/                   # Universal structure and rules
│   ├── time-mechanics.md        # How time works in PrimalMyst
│   ├── dimensional-structure.md # Multiple realities and planes
│   ├── cosmic-forces.md         # Fundamental powers that shape reality
│   └── creation-myths.md        # Origin stories of the universe
├── geography/                   # Physical world structure
│   ├── world-overview.md        # General world description
│   ├── continents/              # Major landmasses
│   ├── regions/                 # Specific areas within continents
│   ├── cities/                  # Major urban centers
│   └── landmarks/               # Notable locations and structures
├── cultures/                    # Civilizations and societies
│   ├── races-and-species.md     # Different intelligent beings
│   ├── nations/                 # Political entities and kingdoms
│   ├── organizations/           # Guilds, orders, and institutions
│   └── social-structures.md     # How societies are organized
├── history/                     # Timeline and historical events
│   ├── ages-and-eras.md         # Major historical periods
│   ├── timeline.md              # mysticlogical event listing
│   ├── wars-and-conflicts.md    # Major battles and struggles
│   └── great-events.md          # World-changing occurrences
├── magic-and-power/             # Supernatural systems
│   ├── magic-systems.md         # How magic works
│   ├── mystical-abilities.md    # Time-related powers
│   ├── artifacts.md             # Magical items and relics
│   └── prophecies.md            # Predictions and their interpretations
└── references/                  # Cross-references and indices
    ├── character-index.md       # Links to character JSON files
    ├── location-index.md        # Links to location JSON files
    ├── event-index.md           # Links to timeline event JSON files
    └── consistency-notes.md     # World-building consistency tracking
```

## Current Documentation Status

### Completed Files
- **playable-races.md** - Comprehensive guide to humanoid heritage, playable races, and the distinction between humanoids and monsters
- **monster-classification-lore.md** - Detailed monster classification system, divine limitations, and exceptional categories (mounts and companions)
- **monster-codex-system.md** - Comprehensive Pokédex-like classification system for cataloging monsters with scientific precision
- **damage-system.md** - Combat mechanics and damage calculations
- **damage-type-interactions.md** - Elemental damage relationships
- **hexagonal-system-applications.md** - Thematic structure applications
- **hexagonal-thematic-structure.md** - Core thematic framework
- **league-system.md** - Game progression and league mechanics

### Key Lore Concepts Documented

#### **Humanoid Heritage System**
- Immutable nature of humanoid heritage (determined at birth, cannot be changed)
- Five playable races: Beast Folk (Canine/Feline), Elfs, and Druids
- All heroes, leaders, and followers must possess humanoid heritage
- Multi-divine influence capability distinguishes humanoids from monsters

#### **The Lost Human Race**
- Original race with five-fingered hands and transcendent potential
- Three theories: Ascension, Annihilation, or Exodus
- Legacy lives on through humanoid heritage in current races

#### **Divine Influence System**
- **Eldritch Pantheon**: Three-tier divine structure (Fundamental, Primal, Veiled)
- **Humanoids**: Can channel multiple divine influences simultaneously
- **Monsters**: Limited to maximum of two divine influences
- Divine limitation creates insurmountable barrier between humanoids and monsters

#### **Monster Classification**
- **Standard Monsters**: All intelligent monsters face divine limitations and social ostracization
- **Mount-Capable Monsters**: Extremely rare (0.1%) with burden-sharing abilities
- **Myrielle-Touched Companions**: Extraordinarily rare (0.01%) guidance providers
- Physical similarity to humanoids doesn't overcome divine limitations

#### **Gameplay Integration**
- Mount system explained through mystical burden-sharing
- Companion system provides lore for HUD enhancements and guidance mechanics
- Divine influence patterns determine character capabilities and social standing

## Writing Guidelines

### Consistency with JSON Data
- All narrative content must align with structured data in `/data/json/`
- Reference JSON IDs when mentioning characters, locations, or events
- Update both narrative and JSON when making changes

### Lore Consistency Rules
- **Divine Influences**: Only reference the Eldritch Pantheon (Pyrion, Glacius, Voltharion, Serafina, Aurelius, Korthak, Myrielle)
- **Humanoid Heritage**: Always immutable, determined at birth, cannot be gained or lost
- **Monster Limitations**: Maximum two divine influences, cannot overcome this barrier
- **Playable Races**: Limited to Beast Folk (Canine/Feline), Elfs, and Druids
- **Social Hierarchy**: Based on divine influence capacity, not prejudice

### Tone and Style
- **Epic Fantasy**: Grand scope with cosmic implications
- **Scholarly**: Present information as discovered knowledge
- **Mysterious**: Leave room for player discovery and interpretation
- **Consistent**: Maintain voice across all documentation

### Content Standards

#### For Official Canonical Content
- Must be approved by the development team
- Clearly marked as canon in metadata
- Follows established lore precedents
- Uses structured templates for consistency

#### For Speculative Content
- Clearly marked as theories or possibilities
- Include multiple interpretations where appropriate
- Note uncertainty and debate among scholars
- Leave room for future development

### Cross-Referencing
- Use consistent naming conventions matching JSON IDs
- Link related concepts across documents
- Maintain bidirectional references (if A mentions B, B should reference A)
- Use tags and categories for easy discovery

## Template Structure

Each world-building document should follow this structure:

```markdown
# [Topic Title]

## Overview
Brief summary of the topic and its importance to the world.

## Key Concepts
Major ideas, rules, or principles that govern this aspect of the world.

## Details
Comprehensive explanation with examples and implications.

## Historical Context
How this developed over time and key historical events.

## Current State
How things stand in the present era of the game.

## Mysteries and Unknowns
Unresolved questions and areas for player discovery.

## Related Elements
- Characters: [List with JSON IDs]
- Locations: [List with JSON IDs]  
- Events: [List with JSON IDs]
- Other Topics: [Cross-references]

## Scholar's Notes
In-world academic perspectives and debates.

## Player Impact
How this affects gameplay and player choices.

## Tags
Searchable keywords for categorization.
```

## Integration with Game Systems

### Data Synchronization
- World-building content informs game mechanics
- JSON data provides structured information for game systems
- Regular audits ensure consistency between narrative and data

### Dynamic Content
- Some elements should remain flexible for player agency
- Mark which aspects can change based on player choices
- Document how player actions might influence the world

### Community Contributions
- Community can contribute theories and interpretations
- Non-canonical speculation enriches the world
- Player discoveries become part of the living lore

## Quality Assurance

### Review Process
1. **Consistency Check**: Verify alignment with existing lore
2. **JSON Validation**: Ensure structured data is properly formatted
3. **Cross-Reference Audit**: Check that all references are valid
4. **Tone Review**: Maintain consistent voice and style
5. **Developer Approval**: Final review for canonical content

### Maintenance
- Regular updates to reflect game development
- Community feedback integration
- Expansion based on player interest and engagement
- Version control for tracking changes

---

*This guide ensures that PrimalMyst's world-building remains consistent, comprehensive, and engaging for both developers and players.*

## Current World-Building Documents

### Game Systems
- [Damage System](./damage-system.md) - Combat mechanics and damage types
- [Damage Type Interactions](./damage-type-interactions.md) - How different damage types affect each other
- [Damage Calculator Reference](./damage-calculator-reference.md) - Mathematical foundations for damage calculation
- [Hexagonal System Applications](./hexagonal-system-applications.md) - Six-element system applications
- [Hexagonal Thematic Structure](./hexagonal-thematic-structure.md) - Thematic foundations of the six-element system
- [League System](./league-system.md) - Player progression and competitive structures

### Racial and Cultural Systems
- [Playable Races](./playable-races.md) - The mystery of the lost Humans and their humanoid descendants

### Data References
- See `/data/json/` for structured lore, character, location, and timeline data
- See `/data/schemas/` for JSON schema definitions



