# Universal Trial System Implementation

**Date:** August 5, 2025  
**Branch:** feature/terminology_gods  
**Purpose:** Create overarching trial category system that groups Myrielle trials and divine trials with centralized world impact mechanics

## Summary

Successfully created a unified trial framework that organizes both Divine Trials and Myrielle's Hidden Trials under a single system while centralizing shared mechanics like tremors and monster level scaling.

## Key Implementation

### 1. Core Framework Created
- **File:** `data/json/trial-system/trial-system-core.json`
- **Purpose:** Central system defining shared mechanics and organizational structure
- **Benefits:** Single source of truth for world impact mechanics

### 2. Trial Categories Established

#### Divine Approval Trials
- **Purpose:** Prove worthiness to exist in divine presence, gain immunity from divine decay
- **Accessibility:** Public knowledge, guild-mediated access
- **Governing Entities:** Six Eldritch Gods (Pyrion, Glacius, Voltharion, Serafina, Aurelius, Korthak)
- **Rewards:** Divine immunity, +6 monster level per trial, social recognition, mystical authority

#### Hidden Cosmic Trials  
- **Purpose:** Prepare worthy souls for cosmic responsibility and God-Slayer status
- **Accessibility:** Secret, requires prerequisites and Myrielle's guidance
- **Governing Entity:** Myrielle (The Hidden One)
- **Rewards:** Ascendency Points, cosmic authority, hidden knowledge, champion preparation

### 3. Shared World Impact Mechanics

#### Divine Acknowledgment Tremor
- **Trigger:** Any trial completion from either category
- **Effects:**
  - Moderate earthquake (45-60 seconds) worldwide
  - +6 minimum monster level increase globally
  - Mystical signature specific to trial type
  - Environmental adaptation to practitioner's power

#### Progressive World Scaling
- **Baseline:** Monsters level 6 after tutorial
- **6 Trials:** Minimum level 36 (end of Act 1)
- **12 Trials:** Minimum level 72 (end of Act 3)
- **Rationale:** World adapts to cosmic authority, incompatible with weaker entities

### 4. File Organization Restructure

#### New Directory Structure
```
data/json/trial-system/
├── trial-system-core.json (central framework)
├── divine-trials/ (moved from divine-trials/)
│   ├── pyrion-forge-trial-of-creation.json
│   ├── glacius-archive-trial-of-preservation.json
│   ├── voltharion-web-trial-of-connection.json
│   ├── serafina-court-trial-of-chaos.json
│   ├── aurelius-sanctuary-trial-of-radiance.json
│   └── korthak-arena-trial-of-might.json
└── myrielle-trials/ (new)
    └── myrielle-hidden-trial-compassion.json (sample)
```

#### Updated References
- **Data Index:** Updated to reflect new organization and schema
- **Individual Trials:** Updated to reference core system for world impact
- **Schema Definitions:** Enhanced to support both trial categories

## Benefits Achieved

### 1. Unified Mechanics
- **Single Source:** All world impact mechanics centralized in core file
- **Consistency:** Both trial types use identical tremor and scaling systems
- **Maintainability:** Changes to world impact only need updates in one location

### 2. Clear Categorization
- **Distinct Purposes:** Divine trials for immunity, Myrielle trials for cosmic preparation
- **Shared Foundation:** Both contribute to cosmic authority through different pathways
- **Progressive Structure:** Divine trials prerequisite for Myrielle trials

### 3. Mystery Preservation
- **Hidden Source:** Myrielle trials trigger same world effects but source is concealed
- **Community Confusion:** People recognize power increase but don't understand origin
- **Political Mystique:** Character gains authority without clear explanation

### 4. Future Expansion Support
- **Framework Flexibility:** Easy to add new trial categories
- **Scaling Adjustments:** World impact can be modified without touching individual trials
- **Cross-Act Integration:** Structure supports trials spanning multiple acts

## Implementation Details

### Core System Features
- **Trial Categories:** Clearly defined divine_trials and myrielle_trials
- **Shared Mechanics:** Centralized Divine Acknowledgment Tremor system
- **Progressive Scaling:** Unified monster level progression tracking
- **Integration Framework:** Prerequisites and progression chains

### Sample Myrielle Trial
- **Created:** `myrielle-hidden-trial-compassion.json`
- **Features:** Moral choice with sacrifice, cosmic transformation rewards
- **Integration:** References core system for world impact mechanics
- **Purpose:** First test of cosmic responsibility and worthiness

### Updated Divine Trial
- **Modified:** `pyrion-forge-trial-of-creation.json`
- **Changes:** Added trial_category field, updated world impact reference
- **Consistency:** Now uses shared tremor system from core framework

## Schema Updates

### New Schemas Needed
- `trial-system.schema.json` - Core framework validation
- `myrielle-trial.schema.json` - Hidden trial structure validation
- Updated `divine-trial.schema.json` - Integration with core system

### Data Index Updates
- Added trial-system category with subcategories
- Updated divine-trial references to new location
- Added myrielle-trial schema definition

## Lore Integration

### Cosmic Significance
- **Unified Purpose:** All trials prepare souls for cosmic responsibility
- **Divine Cooperation:** Divine trials unknowingly serve Myrielle's agenda
- **Reality Preparation:** Progressive scaling prepares world for cosmic conflict
- **Consciousness Preservation:** Ultimate goal of creating transcendent beings

### Mystery Framework
- **Hidden Agenda:** Myrielle trials advance cosmic preparation secretly
- **Divine Ignorance:** Other gods unaware of Myrielle's true purpose
- **Player Discovery:** Gradual revelation of cosmic responsibility theme

## Future Development

### Remaining Myrielle Trials
- **Act 2:** Create remaining 2 hidden trials for Act 2
- **Act 3:** Create 3 ultimate trials for Act 3
- **Progressive Difficulty:** Each trial more demanding than previous

### Advanced Divine Trials
- **Act 2-3:** Enhanced divine trials with cosmic elements
- **Multi-God Scenarios:** Trials requiring multiple divine relationships
- **Conflict Situations:** Trials where divine principles clash

### System Expansion
- **Additional Categories:** Framework supports new trial types
- **Mechanical Refinement:** Tune world impact and scaling as needed
- **Cross-System Integration:** Connect with other hexagonal systems

## Validation

### Mechanical Consistency
- **Tremor System:** Identical effects regardless of trial source
- **Monster Scaling:** Uniform progression across all trial types
- **Authority Accumulation:** Both categories contribute to cosmic standing

### Lore Coherence
- **Divine Purpose:** Divine trials establish foundation for cosmic trials
- **Progressive Preparation:** Each category prepares for the next level
- **Mystery Preservation:** Hidden nature of Myrielle trials maintained

### Technical Implementation
- **File Organization:** Clean separation with shared core
- **Reference Integrity:** All cross-references updated correctly
- **Schema Compliance:** Structure supports validation and tooling

## Conclusion

The Universal Trial System successfully unifies Divine Trials and Myrielle's Hidden Trials under a coherent framework while preserving the mystery and distinct purposes of each category. The centralized world impact mechanics eliminate duplication while ensuring consistent scaling and effects across all trial types.

This implementation provides a solid foundation for future expansion while maintaining clear categorization and progressive difficulty scaling that supports the overarching cosmic responsibility theme of PrimalMyst.
