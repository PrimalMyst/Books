# Hexagonal Thematic Applications for PrimalMyst

## Overview

The core hexagonal structure provides a universal framework for organizing PrimalMyst's systems. This document outlines how to apply the hexagon to various game elements beyond the core damage/god/attribute mappings.

## Core Hexagon Reference

```
                    (1) FIRE 🔴
                   Strength
                 Fire Resistance
                      /\
                     /  \
      (6) SHADOW 🟣    (2) METAL 🟡
        Charisma       Constitution
         Evasion           Armor
                   \    /
                    \  /
      (5) WATER 🔵 ---- (3) AIR 🟢
        Intelligence    Dexterity
       Water Resist   Air Resistance
                    \  /
                     \/
                (4) LIGHTNING 🔷
                    Wisdom
                 Energy Shield
```

## System Applications

### 1. Skill Trees / Passive Trees

**Structure:** Each corner anchors a major branch of the passive skill tree

- **Position 1 (Fire/Str/FR):** Raw damage, fire mastery, physical enhancement, forge arts
- **Position 2 (Metal/Con/Arm):** Weapon mastery, endurance, physical mitigation, martial discipline
- **Position 3 (Air/Dex/AR):** Speed, accuracy, evasion, chain effects, mobility
- **Position 4 (Lightning/Wis/ES):** Divine authority, storm power, spell resistance, healing
- **Position 5 (Water/Int/WR):** Spell power, preservation magic, knowledge, cold immunity
- **Position 6 (Shadow/Cha/Eva):** Stealth, chaos effects, evasion, manipulation

**Connections:** 
- Adjacent corners have direct connection paths (easier to hybrid)
- Opposite corners require travel through intermediary nodes (harder to combine)
- Central hub connects to all six (World Tree mastery)

### 2. Equipment Categories

**Weapons by Corner:**
1. **Fire:** Great swords, War hammers, Two-handed forge weapons
2. **Metal:** Spears, Polearms, Disciplined martial weapons
3. **Air:** Bows, Javelins, Speed weapons
4. **Lightning:** Staves, Divine focuses, Storm implements
5. **Water:** Wands, Crystal tomes, Orbs of knowledge
6. **Shadow:** Daggers, Shadow orbs, Stealth blades

**Armor by Vertex:**
1. **Fire:** Heavy plate with fire resistance bonuses
2. **Metal:** Forged lamellar with armor/endurance hybrid
3. **Air:** Light leather focused on evasion and mobility
4. **Lightning:** Energy-threaded chain with ES/Armor hybrid
5. **Water:** Flowing robes with mana and spell bonuses
6. **Shadow:** Evasion leathers with ES/Evasion hybrid

### 3. Character Classes/Archetypes

**Origin Island Heritage System:**
Character classes inherit their attribute growth patterns from their starting island's hexagonal position:

1. **Warrior (Ifrisurtr's Isle/Position 1):** Strength focus from fire/destruction heritage
2. **Knight (Longares' Isle/Position 2):** Constitution focus from metal/discipline heritage
3. **Hunter (Kitsunrir's Isle/Position 3):** Dexterity focus from air/speed heritage
4. **Sage (Gryphozeus' Isle/Position 4):** Wisdom focus from lightning/authority heritage
5. **Scholar (Tiamangandr's Isle/Position 5):** Intelligence focus from water/preservation heritage
6. **Rogue (Bastenyx's Isle/Position 6):** Charisma focus from shadow/guile heritage

**Class Role - Ascendancy Anchors:**
- Classes provide access to specific ascendancy trees (similar to Path of Exile)
- Each class anchors 3-4 thematic ascendancy specializations
- Multiclass characters can access multiple ascendancy trees through their class combinations
- No hexagonal positioning benefits from classes themselves

**Divine Positioning System:**
- Hexagonal layer positioning comes exclusively from divine trial completion
- 49 unique character archetypes through elemental + primal divine pattern combinations
- Divine positioning independent of character class or origin island
- Players choose their cosmic alignment through trial choices, not class selection

### 4. League Mechanics

**Seasonal Focus:** Each league could emphasize different corners or corner combinations:

- **Ember League:** Focus on fire/destruction and forge crafting mechanics
- **Storm League:** Air/speed emphasis with hunt and evasion mechanics
- **Tidal League:** Water/preservation with enhanced memory and knowledge access
- **Shadow League:** Shadow/stealth with shifting and manipulation mechanics
- **Forge League:** Metal/discipline with combat tournaments and endurance
- **Tribunal League:** Lightning/authority with divine judgment events

**Cross-Vertex Leagues:**
- **Eclipse League:** Opposition pairs (Cold vs Physical, etc.)
- **Harmony League:** Adjacent synergies enhanced
- **World Tree League:** All six corners active simultaneously

### 5. Crafting Materials

**By Vertex Position:**
1. **Fire:** Volcanic Cores, Phoenix Ash, Forge Embers
2. **Metal:** Dragon Scales, Honor Steel, Tempered Alloys
3. **Air:** Storm Feathers, Gale Crystals, Fox-Tail Silk
4. **Lightning:** Thunder Stones, Griffin Talons, Storm Cores
5. **Water:** Abyssal Ice, Memory Crystals, Deep Currents
6. **Shadow:** Moonlit Silk, Sphinx Dust, Twilight Shards

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
