# PrimalMyst Hexagonal Systems - Complete Draft

## Hexagonal Positioning System

### Corner-Based Layout
The PrimalMyst hexagonal system uses **corner positions** rather than edge or face positions. Each corner represents a distinct system element, with **Position 1 at the top** and positions numbered **clockwise** around the hexagon.

### Positional Mapping with Cardinal Directions
```
                    (1) TOP 🔴
                   NORTH CORNER
                   Surtrynix (P)
                      /\
                     /  \
    (6) TOP-LEFT 🟣     (2) TOP-RIGHT 🟡
    NORTHWEST CORNER    NORTHEAST CORNER
    Anubastet (S)       Mavostrax (S)
                   \    /
                    \  /
    (5) BOTTOM-LEFT 🔵 ---- (3) BOTTOM-RIGHT 🟢
    SOUTHWEST CORNER        SOUTHEAST CORNER
    Leviangandr (P)         Kitsunrir (P)
                    \  /
                     \/
                (4) BOTTOM 🔵
                SOUTH CORNER
                Gryphozeus (S)
```

### Position Guidelines
- **Starting Point**: Position 1 is always at the **TOP** (North corner)
- **Direction**: Positions increase **CLOCKWISE** around the hexagon
- **Corner System**: All positions are at **corners**, not edges or faces
- **Cardinal Reference**: Each position has a cardinal/intercardinal direction for spatial clarity

### Position-to-Direction Mapping
| Position | Cardinal Direction | Relative Position | God Tier |
|----------|-------------------|-------------------|----------|
| 1 | North (N) | Top | Primal |
| 2 | Northeast (NE) | Top-Right | Sovereign |
| 3 | Southeast (SE) | Bottom-Right | Primal |
| 4 | South (S) | Bottom | Sovereign |
| 5 | Southwest (SW) | Bottom-Left | Primal |
| 6 | Northwest (NW) | Top-Left | Sovereign |



## Quick Reference Table

| Position/Color | God | Damage Type | Attribute | Armor Type | Resource |
|----------------|-----|-------------|-----------|------------|----------|
| 1 RED 🔴 | Surtrynix | Fire | Strength | *(None)* | Health Points |
| 2 YELLOW 🟡 | Mavostrax | Metal | Constitution | Armor | *(None)* |
| 3 GREEN 🟢 | Kitsunrir | Air | Dexterity | *(None)* | Stamina Points |
| 4 CYAN 🔵 | Gryphozeus | Lightning | Wisdom | Energy Shield | *(None)* |
| 5 BLUE 🔵 | Leviangandr | Water | Intelligence | *(None)* | Mana Points |
| 6 MAGENTA 🟣 | Anubastet | Shadow | Charisma | Evasion | *(None)* |

## Purpose
This document tracks all established hexagonal layers in PrimalMyst and their corner mappings to prepare for full refactoring. Each layer follows the same 6-corner pattern aligned with our RGB color system and divine pantheon structure. All positions use the corner-based clockwise system starting from Position 1 (North/Top) as defined in the Hexagonal Positioning System above.

## Updated Hexagonal Foundation (RGB Anchor System)

### RGB Anchor Structure
The hexagonal system is anchored by the three primary RGB colors at corners 1, 3, and 5, with intermediate corners bridging between them:

```
                    (1) RED 🔴 NORTH
                   Surtrynix (P)
                   Strength
                      /\
                     /  \
(6) MAGENTA NW 🟣        (2) YELLOW NE 🟡
Anubastet (S)            Mavostrax (S)
 Charisma                Constitution
 Evasion                 Armor
                   \    /
                    \  /
(5) BLUE SW 🔵 ---- ---- (3) GREEN SE 🟢
Leviangandr (P)          Kitsunrir (P)
Intelligence             Dexterity
                    \  /
                     \/
                (4) CYAN SOUTH 🔵
                Gryphozeus (S)
                Wisdom
                Energy Shield
```

### RGB Color Anchor System
- **Position 1 (RED)** 🔴 - Primary anchor - Surtrynix (Primal) - Fire damage
- **Position 2 (YELLOW)** 🟡 - Red→Green bridge - Mavostrax (Sovereign) - Red + Green = #FFFF00
- **Position 3 (GREEN)** 🟢 - Primary anchor - Kitsunrir (Primal) - Air damage
- **Position 4 (CYAN)** 🔵 - Green→Blue bridge - Gryphozeus (Sovereign) - Green + Blue = #00FFFF
- **Position 5 (BLUE)** 🔵 - Primary anchor - Leviangandr (Primal) - Water damage
- **Position 6 (MAGENTA)** 🟣 - Blue→Red bridge - Anubastet (Sovereign) - Blue + Red = #FF00FF

**Legend:**
- (P) = Primal God (RGB anchor positions)
- (S) = Sovereign God (bridge positions)

---

## Complete Hexagonal Layer Mapping (RGB Anchor System)

| Position | Color/Theme | God | Tier | Damage Type | Attribute | Armor Type | Resource |
|----------|-------------|-----|------|-------------|-----------|------------|----------|
| 1 | **RED** 🔴 | Surtrynix | Primal | Fire | Strength | *(None)* | Health Points |
| 2 | **YELLOW** 🟡 | Mavostrax | Sovereign | Metal | Constitution | Armor | *(None)* |
| 3 | **GREEN** 🟢 | Kitsunrir | Primal | Air | Dexterity | *(None)* | Stamina Points |
| 4 | **CYAN** 🔵 | Gryphozeus | Sovereign | Lightning | Wisdom | Energy Shield | *(None)* |
| 5 | **BLUE** 🔵 | Leviangandr | Primal | Water | Intelligence | *(None)* | Mana Points |
| 6 | **MAGENTA** 🟣 | Anubastet | Sovereign | Shadow | Charisma | Evasion | *(None)* |

### RGB Anchor Positions
- **Position 1 (RED)**: Primary RGB anchor - Core survival and strength (Fire/Surtrynix)
- **Position 3 (GREEN)**: Primary RGB anchor - Core stamina and dexterity (Air/Kitsunrir)
- **Position 5 (BLUE)**: Primary RGB anchor - Core mana and intelligence (Water/Leviangandr)

---

## Detailed Layer Breakdown

### 1. **Pantheon Layer** (Established)
| Position | God | Full Name | Tier | Domain | Mythological Inspiration |
|----------|-----|-----------|------|--------|-------------------------|
| 1 | Surtrynix | Surtrynix, the Ash Phoenix | Primal | Apocalyptic Fire, Cyclical Rebirth, World-Ending Flame | **Surtr + Phoenix** (Norse/Classical) |
| 2 | Mavostrax | Mavostrax, the Auric Dragon King | Sovereign | Honorable Metal, Disciplined Might, Warrior's Code | **Mars + Dragon King** (Roman/Chinese) |
| 3 | Kitsunrir | Kitsunrir, the Storm-Tailed Hunter | Primal | Monstrous Hunger, Illusory Winds, Oath-Binding Tails | **Fenrir + Nine-Tailed Kitsune** (Norse/Japanese) |
| 4 | Gryphozeus | Gryphozeus, the Thunder Griffin | Sovereign | Divine Authority, Celestial Justice, Holy Lightning | **Zeus + Griffin** (Greek/Classical) |
| 5 | Leviangandr | Leviangandr, the Frozen Coil | Primal | Icy Oceans, Abyssal Pressure, Crystalline Memory | **Leviathan + Jörmungandr** (Hebrew/Norse) |
| 6 | Anubastet | Anubastet, the Veil Sphinx | Sovereign | Afterlife Guidance, Shadow Wisdom, Protective Guardianship | **Anubis + Bastet** (Egyptian) |

#### **Detailed God Descriptions**

**Surtrynix, the Ash Phoenix (Position 1 - Red Fire)**
The primordial fire that ends worlds and begins them anew. Surtrynix fuses the apocalyptic might of the fire-giant with the cyclical rebirth of the phoenix—flame as both ending and promise. A towering titan wreathed in living embers and ash-feathers, Surtrynix swings a blade of starfire while molten wings shed incandescent cinders. Domains: world-ending transformation, purifying destruction, renewal through burning. Surtrynix teaches that endings are sacred, and only in ash can truth be reborn.

**Mavostrax, the Auric Dragon King (Position 2 - Yellow Metal)**
Sovereign of disciplined might and golden law. Mavostrax marries the war-god’s code with the authority of a dragon king—scales like hammered aurum, voice like a legion’s march. He is crowned in lamellar gold and bears a phalanx spearblade. Domains: honorable warfare, metallic perfection, oaths of discipline. Mavostrax teaches that strength without order is waste, and that victory belongs to those who train, endure, and uphold the oath.

**Kitsunrir, the Storm-Tailed Hunter (Position 3 - Green Air)**
The primal gale that hunts with guile. Kitsunrir is a colossal wolf crowned with nine living storm-tails; each tail weaves wind, illusion, and binding oaths. Tornado-song and fox-fire laughter herald the hunt. Domains: boundless appetite, freedom from fetters, trickster winds, oath-scent. Kitsunrir teaches that chains are stories mortals agree to, and that the wild chooses its own path through the storm.

**Gryphozeus, the Thunder Griffin (Position 4 - Cyan Lightning)**
Sovereign arbiter of divine law and sky-borne judgment. Gryphozeus descends as a regal griffin crowned in cyan stormlight, eyes like burning verdicts, voice like thunder over marble courts. Talons sever false bonds; wings cast shields of radiant storm. Domains: divine authority, righteous judgment, protection of the innocent. Gryphozeus teaches that true authority flows from wisdom, and justice must be swift, certain, and tempered with mercy.

**Leviangandr, the Frozen Coil (Position 5 - Blue Water)**
The abyssal serpent whose coils are glaciers and trenches. Leviangandr binds oceans and memories alike—pressure that crushes, ice that preserves, currents that carry knowledge through time. A world-encircling serpent of black water and blue crystal, within whose ice lie trapped songs and histories. Domains: preservation, deep-water might, crystalline memory, tidal magic. Leviangandr teaches that what endures is what is kept, and that depth demands patience.

**Anubastet, the Veil Sphinx (Position 6 - Magenta Shadow)**
Sovereign guide through night and after. Anubastet bears the jackal’s judging gaze and the lioness’s protective grace, crowned in a veil of purple flame. Shadows answer riddles; souls are weighed with kindness and certainty. Domains: death’s thresholds, shadow wisdom, transformative chaos, sanctuary. Anubastet teaches that darkness is not malice but passage, and that change is the mercy by which life continues.

### 2. **Damage Types Layer** (Established)
| Position | Type | Color | Description | Source |
|----------|------|-------|-------------|--------|
| 1 | Fire | 🔴 | Creation-based thermal damage | Primal flame |
| 2 | Metal | 🟡 | Solid force and crushing damage | Raw material strength |
| 3 | Air | 🟢 | Movement-based pressure damage | Elemental flow |
| 4 | Lightning | 🔵 | Electric energy and divine spark | Electrical-divine fusion |
| 5 | Water | 🔵 | Fluid and crystalline damage | Elemental transformation |
| 6 | Shadow | 🟣 | Darkness and reality-warping damage | Absence energy |

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
- **Constitution (Mavostrax)**: "Disciplined Might" - physical conditioning and martial endurance
- **Wisdom (Gryphozeus)**: "Divine Authority, Celestial Justice" - divine wisdom for healing and protection
- **Charisma (Anubastet)**: "Shadow Wisdom, Underworld Order" - charismatic influence spreads change

### 4. **Armor Types Layer** (Implemented)
| Position | Armor Type | Color | Type | Description |
|----------|------------|-------|------|-------------|
| 1 | *(None)* | 🔴 | Primal | Primal gods focus on raw resources, not armor |
| 2 | Armor | 🟡 | Active | Physical damage reduction through equipment |
| 3 | *(None)* | 🟢 | Primal | Primal gods focus on raw resources, not armor |
| 4 | Energy Shield | 🔵 | Active | Mystical barrier absorption |
| 5 | *(None)* | 🔵 | Primal | Primal gods focus on raw resources, not armor |
| 6 | Evasion | 🟣 | Active | Avoiding damage through movement and positioning |

### 5. **Resources Layer** (Updated)
| Position | Resource | RGB Color | Primary Use | Attributes |
|----------|----------|-----------|-------------|------------|
| 1 | Health Points | Red 🔴 | Life force and survival | Strength, Constitution |
| 2 | *(None)* | Yellow 🟡 | Sovereign gods focus on armor types, not resources | - |
| 3 | Stamina Points | Green 🟢 | Physical energy and endurance | Dexterity, Constitution |
| 4 | *(None)* | Cyan 🔵 | Sovereign gods focus on armor types, not resources | - |
| 5 | Mana Points | Blue 🔵 | Magical energy and divine connection | Intelligence, Wisdom |
| 6 | *(None)* | Magenta 🟣 | Sovereign gods focus on armor types, not resources | - |

**Note:** Only RGB anchor positions (1, 3, 5) have core resources - Primal god alignment.
- **Position 1 (Fire/Surtrynix)**: Health represents the vital flame that burns in all living things
- **Position 3 (Air/Kitsunrir)**: Stamina channels wind energy for movement and the endless hunt  
- **Position 5 (Water/Leviangandr)**: Mana flows like frozen streams through crystalline memory

**Armor Type Alignment:** Only bridge positions (2, 4, 6) have armor types - Sovereign god alignment.
- **Position 2 (Metal/Mavostrax)**: Armor provides disciplined protection through metallic defense
- **Position 4 (Lightning/Gryphozeus)**: Energy Shield channels divine authority into protective barriers
- **Position 6 (Shadow/Anubastet)**: Evasion uses shadow wisdom to avoid harm through movement

---

## Implementation Status

### 🚧 **Systems Under Development**
- **Pantheon Layer** - Gods defined, needs lore integration with new system
- **Damage Types Layer** - Basic types established, needs full implementation
- **Attributes Layer** - Core attributes mapped, needs scaling mechanics
- **Armor Types Layer** - Sovereign god alignment established, needs mechanics
- **Resources Layer** - Primal god alignment established, needs scaling formulas

### 📋 **Systems Pending Design**
- **Resistance System** - How damage types interact with defenses
- **Equipment Integration** - How armor types affect gameplay
- **Resource Mechanics** - Regeneration, scaling, and consumption rules
- **Cross-System Interactions** - How layers work together

### 🔧 **Systems Requiring RGB Updates**
- **Color Consistency** - Ensure all emojis and color references are standardized
- **Visual Design** - Update UI elements to match RGB system
- **Documentation** - Align all reference materials with new structure

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
- **Corner positioning**: All positions are at hexagon corners, never edges or faces
- **Position numbering**: Always 1-6, clockwise from top (North corner)
- **Cardinal alignment**: Position 1=North, 2=Northeast, 3=Southeast, 4=South, 5=Southwest, 6=Northwest
- **RGB anchor system**: 1=Red🔴, 3=Green🟢, 5=Blue🔵 are primary anchors
- **Bridge positions**: 2=Yellow🟡, 4=Cyan🔵, 6=Magenta🟣 bridge between RGB anchors
- **Primal/Sovereign alternation**: 1,3,5 = Primal (RGB anchors) | 2,4,6 = Sovereign (bridges)
- **Adjacency benefits**: Neighboring corner positions synergize naturally
- **Opposition challenge**: Opposite corner positions create meaningful tension

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
| 1 | **RED** 🔴 | Surtrynix | Strength & Destruction | Health Points, Fire Damage |
| 3 | **GREEN** 🟢 | Kitsunrir | Dexterity & Gale-Hunt | Stamina Points, Air Damage |
| 5 | **BLUE** 🔵 | Leviangandr | Intelligence & Preservation | Mana Points, Water Damage |

### Bridge Positions (Sovereign Gods)
These three positions create smooth transitions between the RGB anchors:

| Position | Color | God | Bridge Function | Systems Anchored |
|----------|-------|-----|-----------------|------------------|
| 2 | **YELLOW** 🟡 | Mavostrax | Red→Green Bridge | Armor, Metal Damage |
| 4 | **CYAN** 🔵 | Gryphozeus | Green→Blue Bridge | Energy Shield, Lightning Damage |
| 6 | **MAGENTA** 🟣 | Anubastet | Blue→Red Bridge | Evasion, Shadow Damage |

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
