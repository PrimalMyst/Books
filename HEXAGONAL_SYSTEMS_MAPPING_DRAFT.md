# PrimalMyst Hexagonal Systems - Complete Draft

## Master Reference Table

| Position/Color | God | Damage Type | Attribute | Defensive | Resource |
|----------------|-----|-------------|-----------|-----------|----------|
| 1 RED 🔴 | Pyrion | Fire | Strength | Fire Resistance | Health Points |
| 2 YELLOW 🟡 | Korthak | Physical | Constitution | Armor | *(None)* |
| 3 GREEN 🟢 | Voltharion | Lightning | Dexterity | Lightning Resistance | Stamina Points |
| 4 CYAN 🔵 | Aurelius | Radiance | Wisdom | Energy Shield | *(None)* |
| 5 BLUE 🔵 | Glacius | Cold | Intelligence | Cold Resistance | Mana Points |
| 6 MAGENTA 🟣 | Serafina | Chaos | Charisma | Evasion | *(None)* |

## Purpose
This document tracks all established hexagonal layers in PrimalMyst and their corner mappings to prepare for full refactoring. Each layer follows the same 6-position pattern aligned with our RGB color system and divine pantheon structure.

## Updated Hexagonal Foundation (RGB Anchor System)

### RGB Anchor Structure
The hexagonal system is anchored by the three primary RGB colors at positions 1, 3, and 5, with intermediate positions bridging between them:

```
                    (1) RED 🔴
                   Pyrion (P)
                   Strength
                      /\
                     /  \
         (6) MAGENTA     (2) YELLOW
         Serafina (S)    Korthak (S)
          Charisma       Constitution
        Evasion          Armor
                   \    /
                    \  /
         (5) BLUE 🔵 ---- ---- (3) GREEN 🟢
         Glacius (P)         Voltharion (P)
         Intelligence        Dexterity
                    \  /
                     \/
                (4) CYAN
                Aurelius (S)
                Wisdom
                Energy Shield
```

### RGB Color Anchor System
- **Position 1 (RED)** 🔴 - Primary anchor - Pyrion (Primal) - Fire damage
- **Position 2 (YELLOW)** � - Red→Green bridge - Serafina (Sovereign) - Red + Green = #FFFF00
- **Position 3 (GREEN)** 🟢 - Primary anchor - Voltharion (Primal) - Lightning damage
- **Position 4 (CYAN)** � - Green→Blue bridge - Korthak (Sovereign) - Green + Blue = #00FFFF
- **Position 5 (BLUE)** 🔵 - Primary anchor - Glacius (Primal) - Cold damage
- **Position 6 (MAGENTA)** � - Blue→Red bridge - Aurelius (Sovereign) - Blue + Red = #FF00FF

**Legend:**
- (P) = Primal God (RGB anchor positions)
- (S) = Sovereign God (bridge positions)

---

## Complete Hexagonal Layer Mapping (RGB Anchor System)

| Position | Color/Theme | God | Tier | Damage Type | Attribute | Offensive | Defensive | Resource |
|----------|-------------|-----|------|-------------|-----------|-----------|-----------|----------|
| 1 | **RED** 🔴 | Pyrion | Primal | Fire | Intelligence | Precision Strikes | Fire Resistance | Health Points |
| 2 | **YELLOW** � | Serafina | Sovereign | Chaos | Adaptability | Unpredictable Assault | Evasion | *(None)* |
| 3 | **GREEN** 🟢 | Voltharion | Primal | Lightning | Dexterity | Speed Dominance | Lightning Resistance | Mana Points |
| 4 | **CYAN** � | Korthak | Sovereign | Physical | Strength | Physical Overwhelm | Armor | *(None)* |
| 5 | **BLUE** 🔵 | Glacius | Primal | Cold | Vitality | Burst Devastation | Cold Resistance | Stamina Points |
| 6 | **MAGENTA** � | Aurelius | Sovereign | Radiance | Wisdom | Sustained Mastery | Energy Shield | *(None)* |

### RGB Anchor Positions
- **Position 1 (RED)**: Primary RGB anchor - Core survival and strength (Fire/Pyrion)
- **Position 3 (GREEN)**: Primary RGB anchor - Core stamina and dexterity (Lightning/Voltharion)
- **Position 5 (BLUE)**: Primary RGB anchor - Core mana and intelligence (Cold/Glacius)

---

## Detailed Layer Breakdown

### 1. **Pantheon Layer** (Established)
| Position | God | Full Name | Tier | Domain |
|----------|-----|-----------|------|--------|
| 1 | Pyrion | Pyrion, the First Flame | Primal | Creation, Transformation, Energy Generation |
| 2 | Korthak | Korthak, the Dragon King | Sovereign | Honorable Strength, Disciplined Might |
| 3 | Voltharion | Voltharion, the Cosmic Spark | Primal | Connection, Communication, Divine Revelation |
| 4 | Aurelius | Aurelius, the Radiant Sphere | Sovereign | Healing Light, Protective Order |
| 5 | Glacius | Glacius, the Eternal Frost | Primal | Preservation, Memory, Structural Stability |
| 6 | Serafina | Serafina, the Shadow Empress | Sovereign | Beneficial Chaos, Creative Revolution |

### 2. **Damage Types Layer** (Established)
| Position | Type | Color | Description | Source |
|----------|------|-------|-------------|--------|
| 1 | Fire | 🔴 | Creation-based thermal damage | Primal flame |
| 2 | Physical | � | Direct force and impact damage | Raw might and strength |
| 3 | Lightning | 🟢 | Connection-based electrical damage | Divine spark |
| 4 | Radiance | � | Divine light and truth damage | Protective purification |
| 5 | Cold | 🔵 | Preservation-based crystalline damage | Eternal frost |
| 6 | Chaos | � | Unpredictable, reality-warping damage | Transformation energy |

### 3. **Attributes Layer** (Implemented)
| Position | Attribute | Type | Description | Scaling |
|----------|-----------|------|-------------|---------|
| 1 | Strength | Pure | Physical power and might | Physical damage, health |
| 2 | Constitution | Hybrid | Physical resilience and endurance | Health, armor effectiveness, stamina regeneration |
| 3 | Dexterity | Pure | Speed, accuracy, and precision | Attack speed, accuracy |
| 4 | Wisdom | Hybrid | Applied knowledge and divine insight | Spell resistance, healing power, energy shield |
| 5 | Intelligence | Pure | Mental acuity and magical understanding | Spell power, mana |
| 6 | Charisma | Hybrid | Social influence and force of personality | Chaos effects, manipulation, luck |

#### **Attribute Design Logic**
**RGB Anchors (Pure Attributes):**
- **Strength (Position 1)**: Core physical power - foundation of health and physical damage
- **Dexterity (Position 3)**: Core agility - foundation of stamina and precise action  
- **Intelligence (Position 5)**: Core mental power - foundation of mana and magical understanding

**Bridge Attributes (Classic RPG Stats):**
- **Constitution (Position 2)**: Bridges Strength→Dexterity through physical conditioning and endurance
- **Wisdom (Position 4)**: Bridges Dexterity→Intelligence through applied knowledge and divine insight
- **Charisma (Position 6)**: Bridges Intelligence→Strength through force of personality and social influence

**God Alignment:**
- **Constitution (Korthak)**: "Disciplined Might" - physical conditioning and martial endurance
- **Wisdom (Aurelius)**: "Healing Light, Protective Order" - divine wisdom for healing and protection
- **Charisma (Serafina)**: "Beneficial Chaos, Creative Revolution" - charismatic influence spreads change

### 4. **Offensive Layers** (Implemented)
| Position | Style | Description | Focus |
|----------|-------|-------------|-------|
| 1 | Precision Strikes | Targeted attacks with perfect calculation | Critical hits, weakpoint exploitation |
| 2 | Unpredictable Assault | Chaotic combat that confuses enemies | Adaptive tactics, chaos effects |
| 3 | Speed Dominance | Overwhelming through superior speed | Multi-hit, movement-based attacks |
| 4 | Sustained Mastery | Reliable consistent force | Sustained DPS, defensive offense |
| 5 | Burst Devastation | Explosive decisive moments | Area damage, transformation effects |
| 6 | Physical Overwhelm | Raw might crushing opposition | High damage, direct confrontation |

### 5. **Defensive Layers** (Implemented)
| Position | Defense | Color | Type | Description |
|----------|---------|-------|------|-------------|
| 1 | Fire Resistance | 🔴 | Elemental | Pure immunity to fire damage |
| 2 | Armor | � | Active | Physical damage reduction through equipment |
| 3 | Lightning Resistance | 🟢 | Elemental | Pure immunity to lightning damage |
| 4 | Energy Shield | � | Active | Mystical barrier absorption |
| 5 | Cold Resistance | 🔵 | Elemental | Pure immunity to cold damage |
| 6 | Evasion | � | Active | Avoiding damage through movement and positioning |

### 6. **Resources Layer** (Updated)
| Position | Resource | RGB Color | Primary Use | Attributes |
|----------|----------|-----------|-------------|------------|
| 1 | Health Points | Red 🔴 | Life force and survival | Strength, Constitution |
| 3 | Stamina Points | Green 🟢 | Physical energy and endurance | Dexterity, Constitution |
| 5 | Mana Points | Blue 🔵 | Magical energy and divine connection | Intelligence, Wisdom |

**Note:** Only RGB anchor positions (1, 3, 5) have core resources.
- **Position 1 (Fire/Pyrion)**: Health represents the vital flame of life
- **Position 3 (Lightning/Voltharion)**: Stamina channels electrical energy for endurance  
- **Position 5 (Cold/Glacius)**: Mana preserves magical knowledge through crystalline memory

---

## Implementation Status

### ✅ **Fully Implemented Systems**
- **Pantheon Layer** - All 6 gods defined with complete lore
- **Attributes Layer** - All 6 attributes with scaling and mechanics
- **Offensive Layers** - All 6 combat styles defined
- **Defensive Layers** - All 6 defense types implemented
- **Resources Layer** - 3 core resources mapped to RGB positions

### 🔧 **Systems Requiring RGB Updates**
- **Damage Types** - Need to update from elemental names to RGB colors
- **Color Themes** - Update visual design to match RGB system
- **Hexagonal Structure Diagrams** - Update all documentation

### 📋 **Potential Future Layers**
Based on the established pattern, additional hexagonal systems could include:

#### Equipment Types
| Position | Weapon Type | Armor Type | Jewelry Type |
|----------|-------------|------------|--------------|
| 1 | Staves/Wands | Cloth/Robes | Memory Crystals |
| 2 | Daggers/Orbs | Light/Leather | Chaos Charms |
| 3 | Bows/Javelins | Medium/Chain | Speed Rings |
| 4 | Swords/Axes | Heavy/Plate | Might Amulets |
| 5 | Hammers/Mauls | Forge/Scale | Creation Gems |
| 6 | Shields/Maces | Sacred/Blessed | Protection Wards |

#### Environmental Zones
| Position | Zone Type | Theme | Mechanics |
|----------|-----------|-------|-----------|
| 1 | Crystalline Archives | Preservation | Memory enhancement, knowledge access |
| 2 | Shadow Courts | Transformation | Reality shifting, chaos effects |
| 3 | Lightning Webs | Connection | Fast travel, communication |
| 4 | Combat Arenas | Honor | Physical challenges, fair combat |
| 5 | Creation Forges | Crafting | Item creation, enhancement |
| 6 | Sacred Sanctuaries | Protection | Healing, divine favor |

#### Skill Trees
| Position | Skill Tree | Focus | Examples |
|----------|------------|-------|----------|
| 1 | Preservation Mastery | Memory, Knowledge | Perfect Recall, Time Lock |
| 2 | Chaos Arts | Transformation | Shape Change, Reality Warp |
| 3 | Connection Weaving | Speed, Communication | Instant Travel, Divine Link |
| 4 | Might Disciplines | Strength, Honor | Perfect Strike, Unbreakable |
| 5 | Creation Forces | Energy, Crafting | Material Genesis, Life Spark |
| 6 | Radiance Mysteries | Protection, Truth | Divine Shield, Absolute Truth |

---

## Cross-System Relationships

### Adjacency Synergies (Natural Combinations)
- **1↔2**: Strength + Constitution = **Unstoppable Endurance**
- **2↔3**: Constitution + Dexterity = **Athletic Mastery**  
- **3↔4**: Dexterity + Wisdom = **Perfect Awareness**
- **4↔5**: Wisdom + Intelligence = **Scholarly Mastery**
- **5↔6**: Intelligence + Charisma = **Persuasive Genius**
- **6↔1**: Charisma + Strength = **Commanding Presence**

### Opposition Tensions (Challenging Combinations)
- **1↔4**: Strength vs Wisdom = **Raw Power vs Applied Knowledge**
- **2↔5**: Constitution vs Intelligence = **Physical Endurance vs Mental Agility**
- **3↔6**: Dexterity vs Charisma = **Precise Action vs Social Influence**

---

## Refactoring Priorities

### High Priority (Core Systems)
1. **Update Damage Types** - Convert Cold/Lightning/Fire → Red/Green/Blue
2. **Resource System Integration** - Ensure RGB alignment is consistent
3. **Pantheon References** - Update all Primal/Sovereign trio references
4. **Color Theme Updates** - Visual consistency across all systems

### Medium Priority (Expansion Systems)
1. **Equipment Layer Development** - Create hexagonal equipment system
2. **Environmental Zone Mapping** - Align world areas with hexagonal structure
3. **Skill Tree Architecture** - Implement hexagonal passive trees

### Low Priority (Polish)
1. **Documentation Updates** - Ensure all files reflect new structure
2. **Cross-Reference Validation** - Verify all links work correctly
3. **Schema Compliance** - Update JSON schemas for new structure

---

## Design Principles Maintained

### Consistency Rules
- **Position numbering**: Always 1-6, clockwise from top
- **RGB anchor system**: 1=Red🔴, 3=Green🟢, 5=Blue🔵 are primary anchors
- **Bridge positions**: 2=Yellow�, 4=Cyan�, 6=Magenta� bridge between RGB anchors
- **Primal/Sovereign alternation**: 1,3,5 = Primal (RGB anchors) | 2,4,6 = Sovereign (bridges)
- **Adjacency benefits**: Neighboring positions synergize naturally
- **Opposition challenge**: Opposite positions create meaningful tension

### Thematic Coherence
- **Divine alignment**: All systems reflect corresponding god's nature
- **Cosmic logic**: Mechanics reinforce lore and world-building
- **Player intuition**: Patterns become learnable and predictable
- **Strategic depth**: Multiple viable paths with clear trade-offs

---

## RGB Anchor System Design

### Primary RGB Anchors (Primal Gods)
These three positions form the foundational triangle of the hexagonal system:

| Position | Color | God | Role | Systems Anchored |
|----------|-------|-----|------|------------------|
| 1 | **RED** 🔴 | Pyrion | Strength & Creation | Health Points, Fire Damage, Fire Resistance |
| 3 | **GREEN** 🟢 | Voltharion | Dexterity & Connection | Stamina Points, Lightning Damage, Lightning Resistance |
| 5 | **BLUE** 🔵 | Glacius | Intelligence & Preservation | Mana Points, Cold Damage, Cold Resistance |

### Bridge Positions (Sovereign Gods)
These three positions create smooth transitions between the RGB anchors:

| Position | Color | God | Bridge Function | Color Blend |
|----------|-------|-----|-----------------|-------------|
| 2 | **YELLOW** � | Serafina | Red→Green Bridge | Red + Green = #FFFF00 |
| 4 | **CYAN** � | Korthak | Green→Blue Bridge | Green + Blue = #00FFFF |
| 6 | **MAGENTA** � | Aurelius | Blue→Red Bridge | Blue + Red = #FF00FF |

### Color Wheel Logic
The hexagonal positions follow natural color wheel progression:
- **RGB Primaries** at positions 1, 3, 5 create the foundational triangle
- **Secondary Colors** at positions 2, 4, 6 bridge between primaries
- **Clockwise flow** maintains color harmony: Red→Yellow→Green→Cyan→Blue→Magenta→Red

### System Integration Benefits
1. **Visual Coherence** - UI elements can use consistent color coding
2. **Intuitive Learning** - Players naturally understand color relationships
3. **Thematic Resonance** - Gods embody their color's properties
4. **Mechanical Balance** - RGB anchors provide core systems, bridges add complexity

---

*This draft serves as the foundation for systematic refactoring of all hexagonal systems to ensure consistency, RGB color integration, and maintained thematic coherence throughout PrimalMyst.*
