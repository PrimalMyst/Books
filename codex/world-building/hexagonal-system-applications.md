# Hexagonal Thematic Applications for PrimalMyst

## Overview

The core hexagonal structure provides a universal framework for organizing PrimalMyst's systems. This document outlines how to apply the hexagon to various game elements beyond the core damage/god/attribute mappings.

## Core Hexagon Reference

```
                    (1) COLD
                   Intelligence
                 Cold Resistance
                      /\
                     /  \
         (6) RADIANCE    (2) CHAOS
          Str + Int      Int + Dex
        Energy Shield     Evasion
                   \    /
                    \  /
         (5) FIRE ---- ---- (3) LIGHTNING
         Strength           Dexterity  
         Fire Resist    Lightning Resist
                    \  /
                     \/
                (4) PHYSICAL
                Dex + Str
                Armor
```

## System Applications

### 1. Skill Trees / Passive Trees

**Structure:** Each corner anchors a major branch of the passive skill tree

- **Position 1 (Cold/Int/CR):** Spell power, mana, cold immunity, preservation magic
- **Position 2 (Chaos/Int+Dex/Eva):** Chaos magic, hybrid casting, evasive transformation
- **Position 3 (Lightning/Dex/LR):** Speed, accuracy, lightning immunity, chain effects, mobility
- **Position 4 (Physical/Dex+Str/Arm):** Weapon mastery, martial arts, physical mitigation
- **Position 5 (Fire/Str/FR):** Raw damage, fire immunity, physical enhancement
- **Position 6 (Radiance/Str+Int/ES):** Protection, healing, energy shield mastery

**Connections:** 
- Adjacent corners have direct connection paths (easier to hybrid)
- Opposite corners require travel through intermediary nodes (harder to combine)
- Central hub connects to all six (World Tree mastery)

### 2. Equipment Categories

**Weapons by Corner:**
1. **Cold:** Staves, Wands, Crystal Focuses
2. **Chaos:** Ritual Daggers, Transformation Orbs, Entropy Weapons  
3. **Lightning:** Javelins, Crossbows, Speed Weapons
4. **Physical:** Swords, Axes, Martial Arts Weapons
5. **Fire:** Two-handed weapons, Hammers, Forge Weapons
6. **Radiance:** Shields, Maces, Protective Weapons

**Armor by Vertex:**
1. **Cold:** Robes, Cloth armor with ES bonuses
2. **Chaos:** Light armor with ES/Evasion hybrid
3. **Lightning:** Light armor focused on evasion and mobility
4. **Physical:** Medium armor with evasion/armor hybrid
5. **Fire:** Heavy armor with maximum protection
6. **Radiance:** Heavy armor with armor/ES hybrid

### 3. Character Classes/Archetypes

**Pure Vertex Classes:**
1. **Frost Mage (Cold):** Pure intelligence caster
2. **Lightning Dancer (Lightning):** Pure dexterity speed fighter
3. **Fire Warrior (Fire):** Pure strength heavy combat

**Hybrid Vertex Classes:**
2. **Chaos Weaver (Chaos):** Int/Dex hybrid mage-rogue
4. **Dragon Monk (Physical):** Dex/Str hybrid martial artist  
6. **Radiant Paladin (Radiance):** Str/Int hybrid warrior-priest

### 4. League Mechanics

**Seasonal Focus:** Each league could emphasize different corners or corner combinations:

- **Glacial League:** Focus on cold/preservation mechanics
- **Storm League:** Lightning/speed emphasis with chain reactions
- **Forge League:** Fire/creation with enhanced crafting
- **Shadow League:** Chaos/transformation with shifting mechanics
- **Arena League:** Physical/honor with combat tournaments
- **Sanctuary League:** Radiance/protection with safe zone mechanics

**Cross-Vertex Leagues:**
- **Eclipse League:** Opposition pairs (Cold vs Physical, etc.)
- **Harmony League:** Adjacent synergies enhanced
- **World Tree League:** All six corners active simultaneously

### 5. Crafting Materials

**By Vertex Position:**
1. **Cold:** Eternal Ice, Memory Crystals, Preservation Essences
2. **Chaos:** Shadow Silk, Transformation Catalysts, Entropy Shards
3. **Lightning:** Storm Cores, Speed Crystals, Connection Wires
4. **Physical:** Dragon Scales, Honor Steel, Discipline Stones
5. **Fire:** Flame Hearts, Creation Embers, Forge Coals
6. **Radiance:** Light Gems, Protection Wards, Truth Crystals

**Combination Materials:**
- Adjacent combinations create enhanced materials
- Opposite combinations create rare, challenging-to-use materials
- Full-spectrum materials (all six) create legendary components

### 6. Quest Design

**Vertex-Focused Questlines:**
- Each major questline explores one vertex theme deeply
- Adjacent quests can be done in either order with different outcomes
- Opposite quests create narrative tension and meaningful choices

**Cross-Vertex Narratives:**
- Story arcs that require understanding multiple corners
- Character development that spans the hexagon
- Endgame content that tests mastery of all six themes

### 7. PvP Balance

**Rock-Paper-Scissors Dynamics:**
- Adjacent elements have slight advantages over each other
- Opposite elements create hard counters that require adaptation
- Pure builds excel in specific situations
- Hybrid builds offer versatility but less specialization

**Arena Design:**
- Six-sided battle arenas reflecting the hexagon
- Environmental effects that rotate through the six elements
- Victory conditions that favor different vertex approaches

### 8. Boss Design

**Single-Vertex Bosses:**
- Each boss embodies one vertex perfectly
- Requires understanding of that vertex's strengths/weaknesses
- Can be approached effectively by opposite vertex builds

**Multi-Vertex Bosses:**
- Bosses that shift between adjacent corners
- Requires adaptability and hybrid approaches
- Elite bosses that cycle through all six corners

**Endgame Encounters:**
- World Tree bosses that test mastery of all six vertices
- Raids requiring teams with complementary vertex specializations

### 9. Economy Design

**Resource Distribution:**
- Each vertex produces specific types of resources
- Trade networks follow hexagonal adjacency patterns
- Economic cycles that emphasize different vertices seasonally

**Currency Types:**
- Basic currencies aligned with each vertex
- Exchange rates that reflect adjacency relationships
- Premium currencies for cross-vertex transactions

### 10. Guild Systems

**Guild Specializations:**
- Guilds can choose vertex specializations for bonuses
- Adjacent guild alliances for mutual benefits
- Cross-vertex guild conflicts for territorial control

**Guild Halls:**
- Six-winged hall designs reflecting the hexagon
- Specialized facilities for each vertex
- Central hub for World Tree mastery activities

## Implementation Guidelines

### Design Principles

1. **Consistency:** Always respect the hexagonal relationships
2. **Balance:** Ensure no single vertex dominates
3. **Synergy:** Adjacent elements should feel natural together
4. **Tension:** Opposite elements should create meaningful choices
5. **Progression:** Allow advancement from pure → hybrid → mastery builds

### Content Creation Checklist

When creating new content, ask:
- [ ] Which vertex does this primarily serve?
- [ ] How does it interact with adjacent vertices?
- [ ] Does it create interesting dynamics with opposite vertices?
- [ ] Can it contribute to World Tree mastery builds?
- [ ] Does it maintain hexagonal balance?

### Player Communication

- Use consistent visual language (colors, symbols) for each vertex
- Teach the hexagon gradually through gameplay, not exposition
- Make adjacency benefits and opposition challenges clear through mechanics
- Reward players who understand and utilize the hexagonal relationships

This hexagonal framework ensures that all PrimalMyst systems connect meaningfully while maintaining the cosmic balance that defines the game's universe.
