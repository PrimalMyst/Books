# Main Story Data Files

This folder contains all the structured data files that define PrimalMyst's main storyline progression across all acts.

## Content Organization

### Story Progression Files
- **`prologue-awakening-journey.json`** - Tutorial island and character awakening
- **`act1-divine-trials.json`** - Divine trials and positioning establishment (levels 10-39)
- **`act2-eldritch-ascension.json`** - Eldritch mysteries and cosmic understanding (levels 40-69)
- **`act3-cosmic-ascendant.json`** - Divine mastery and champion status (levels 70-84)
- **`epilogue-god-slayer-ascension.json`** - Divine confrontations and transcendence (levels 85-100)

### Framework Files
- **`act-level-rank-structure.json`** - Canonical definition of level/rank/act relationships
- **`primalmyst-story-structure.json`** - Overall story framework and progression systems

## Schema Compliance

All files in this folder follow the `lore.schema.json` structure and contain:
- Unique ID-based references for cross-linking
- Canonical progression information
- Level/rank gating requirements
- Story beats and narrative structure

## Integration

These files integrate with:
- **Codex Documentation**: Referenced by markdown files in `codex/lore/`
- **Game Systems**: Provide progression gates and content access rules
- **Data Index**: Catalogued in `data/index.json` under the `main-story` category

## Purpose

This organization separates the core storyline progression from general world lore, making it easier to:
- Track multi-act narrative development
- Manage progression system updates
- Coordinate story-related content changes
- Provide canonical references for story structure

## Related Content

For additional story context, see:
- `codex/lore/` - Narrative documentation
- `data/json/lore/` - General world lore and systems
- `data/schemas/lore.schema.json` - Data structure definitions
