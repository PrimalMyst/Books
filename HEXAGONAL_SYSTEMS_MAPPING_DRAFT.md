# PrimalMyst Hexagonal Systems - Complete Draft



## Quick Reference Table

| Position/Color | God | Damage Type | Attribute | Armor Type | Resource |
|----------------|-----|-------------|-----------|------------|----------|
| 1 RED 🔴 | Surturon | Fire | Strength | *(None)* | Health Points |
| 2 YELLOW 🟡 | Marsalis | Metal | Constitution | Armor | *(None)* |
| 3 GREEN 🟢 | Fenrion | Air | Dexterity | *(None)* | Stamina Points |
| 4 CYAN 🔵 | Zeusara | Lightning | Wisdom | Energy Shield | *(None)* |
| 5 BLUE 🔵 | Jormunion | Water | Intelligence | *(None)* | Mana Points |
| 6 MAGENTA 🟣 | Anubiseth | Shadow | Charisma | Evasion | *(None)* |

## Purpose
This document tracks all established hexagonal layers in PrimalMyst and their corner mappings to prepare for full refactoring. Each layer follows the same 6-position pattern aligned with our RGB color system and divine pantheon structure.

## Updated Hexagonal Foundation (RGB Anchor System)

### RGB Anchor Structure
The hexagonal system is anchored by the three primary RGB colors at positions 1, 3, and 5, with intermediate positions bridging between them:

```
                    (1) RED 🔴
                   Surturon (P)
                   Strength
                      /\
                     /  \
         (6) MAGENTA     (2) YELLOW
         Anubiseth (S)   Marsalis (S)
          Charisma       Constitution
        Evasion          Armor
                   \    /
                    \  /
         (5) BLUE 🔵 ---- ---- (3) GREEN 🟢
         Jormunion (P)        Fenrion (P)
         Intelligence        Dexterity
                    \  /
                     \/
                (4) CYAN
                Zeusara (S)
                Wisdom
                Energy Shield
```

### RGB Color Anchor System
- **Position 1 (RED)** 🔴 - Primary anchor - Surturon (Primal) - Fire damage
- **Position 2 (YELLOW)** 🟡 - Red→Green bridge - Marsalis (Sovereign) - Red + Green = #FFFF00
- **Position 3 (GREEN)** 🟢 - Primary anchor - Fenrion (Primal) - Air damage
- **Position 4 (CYAN)** 🔵 - Green→Blue bridge - Zeusara (Sovereign) - Green + Blue = #00FFFF
- **Position 5 (BLUE)** 🔵 - Primary anchor - Jormunion (Primal) - Water damage
- **Position 6 (MAGENTA)** 🟣 - Blue→Red bridge - Anubiseth (Sovereign) - Blue + Red = #FF00FF

**Legend:**
- (P) = Primal God (RGB anchor positions)
- (S) = Sovereign God (bridge positions)

---

## Complete Hexagonal Layer Mapping (RGB Anchor System)

| Position | Color/Theme | God | Tier | Damage Type | Attribute | Armor Type | Resource |
|----------|-------------|-----|------|-------------|-----------|------------|----------|
| 1 | **RED** 🔴 | Surturon | Primal | Fire | Strength | *(None)* | Health Points |
| 2 | **YELLOW** 🟡 | Marsalis | Sovereign | Metal | Constitution | Armor | *(None)* |
| 3 | **GREEN** 🟢 | Fenrion | Primal | Air | Dexterity | *(None)* | Stamina Points |
| 4 | **CYAN** 🔵 | Zeusara | Sovereign | Lightning | Wisdom | Energy Shield | *(None)* |
| 5 | **BLUE** 🔵 | Jormunion | Primal | Water | Intelligence | *(None)* | Mana Points |
| 6 | **MAGENTA** 🟣 | Anubiseth | Sovereign | Shadow | Charisma | Evasion | *(None)* |

### RGB Anchor Positions
- **Position 1 (RED)**: Primary RGB anchor - Core survival and strength (Fire/Surturon)
- **Position 3 (GREEN)**: Primary RGB anchor - Core stamina and dexterity (Air/Fenrion)
- **Position 5 (BLUE)**: Primary RGB anchor - Core mana and intelligence (Water/Jormunion)

---

## Detailed Layer Breakdown

### 1. **Pantheon Layer** (Established)
| Position | God | Full Name | Tier | Domain | Mythological Inspiration |
|----------|-----|-----------|------|--------|-------------------------|
| 1 | Surturon | Surturon, the World-Ending Flame | Primal | Apocalyptic Fire, World Destruction, Ragnarök | **Surtr** (Norse) - Fire giant who will burn all nine worlds at Ragnarök |
| 2 | Marsalis | Marsalis, the Golden Dragon | Sovereign | Honorable Metal, Disciplined Might, Warrior's Way | **Mars** (Roman) - God of war and military strategy |
| 3 | Fenrion | Fenrion, the Devouring Wind | Primal | Monstrous Hunger, Boundless Growth, Wind-Carried Howls | **Fenrir** (Norse) - Monstrous wolf destined to devour Odin at Ragnarök |
| 4 | Zeusara | Zeusara, the Divine Thunder | Sovereign | Holy Lightning, Divine Authority, Celestial Justice | **Zeus** (Greek) - King of gods, ruler of sky and thunder |
| 5 | Jormunion | Jormunion, the Frozen Depths | Primal | Icy Oceans, Crushing Depths, Frozen Memory | **Jörmungandr** (Norse) - World Serpent who encircles Midgard in the ocean |
| 6 | Anubiseth | Anubiseth, the Shadow Judge | Sovereign | Afterlife Guidance, Shadow Wisdom, Underworld Order | **Anubis** (Egyptian) - Jackal-headed god of the afterlife and mummification |

#### **Detailed God Descriptions**

**Surturon, the World-Ending Flame (Position 1 - Red Fire)**
The primordial god of apocalyptic destruction and world-ending transformation, Surturon embodies the essential fire that will consume all existence at the end of times. As the World-Ending Flame, he represents the inevitable conclusion of all cycles - the fire that burns away everything to make space for what comes next. Surturon's domain encompasses not just destructive fire, but the necessary apocalyptic force that cleanses reality for rebirth. He appears as a towering figure of living flame wielding a massive flaming sword, his form constantly crackling with world-consuming energy. Surturon teaches that all things must end so that new things can begin, and that destruction is not evil but necessary. His followers are revolutionaries, those who seek to tear down corrupt systems, and anyone who understands that sometimes everything must burn for truth to emerge. **Inspired by Surtr, the Norse fire giant destined to burn all nine worlds at Ragnarök.**

**Marsalis, the Golden Dragon (Position 2 - Yellow Metal)**
The sovereign god of honorable warfare and metallic perfection, Marsalis embodies the warrior's path through disciplined might and golden virtue. As the Golden Dragon, he represents the fusion of draconic power with Roman military discipline - strength tempered by honor and tactical excellence. Marsalis appears as a magnificent humanoid dragon wreathed in golden scales and radiant armor, wielding weapons of pure celestial metal. His domain covers not just physical combat, but the forging of character through discipline, the creation of perfect weapons and armor, and the warrior's code that turns mere fighting into noble art. He teaches that true strength comes from self-mastery and disciplined training, and that the greatest victories are won through honor, strategy, and unwavering dedication to the warrior's way. **Inspired by Mars, the Roman god of war and military strategy.**

**Fenrion, the Devouring Wind (Position 3 - Green Air)**
The primal god of monstrous hunger and unstoppable growth, Fenrion represents the terrible power of appetite that can never be satisfied. As the Devouring Wind, he embodies the howling gales that carry his endless hunger across all realms, growing larger and more powerful with everything he consumes. Fenrion appears as a massive spectral wolf whose form is made of swirling winds and storm clouds, his howls echoing across vast distances as tornadoes dance around his ethereal figure. His domain encompasses boundless appetite, the power that breaks all chains, the wind that carries terror, and the hunger that grows stronger the more it feeds. He teaches that all bonds are temporary, that growth requires consumption, and that even the gods cannot contain what is destined to be free. His followers are those who refuse to be bound, rebels against authority, and anyone who understands that sometimes appetite is stronger than law. **Inspired by Fenrir, the monstrous Norse wolf destined to break free and devour Odin at Ragnarök.**

**Zeusara, the Divine Thunder (Position 4 - Cyan Lightning)**
The sovereign goddess of divine authority and celestial justice, Zeusara wields the power of holy lightning to enforce cosmic law and divine will. As the Divine Thunder, she represents the awesome power of divine judgment made manifest through electrical storms and thunderous proclamations. Zeusara appears as a regal figure wreathed in cyan lightning, her voice carrying the authority of thunder itself, her eyes blazing with the light of divine justice. Her domain covers divine law, righteous judgment, the protection of the innocent, and the punishment of the wicked. She teaches that true authority comes from wisdom rather than force, and that justice must be swift, certain, and tempered with mercy. **Inspired by Zeus, the Greek king of gods and ruler of sky and thunder.**

**Jormunion, the Frozen Depths (Position 5 - Blue Water)**
The primal god of icy preservation and crushing depths, Jormunion embodies the power to freeze, preserve, and crush through the terrible pressure of the deepest waters. As the Frozen Depths, he represents the endless cycle of ice and water - from frozen memories locked in glacial ice to the crushing pressure of ocean depths that can destroy anything. Jormunion appears as a massive serpentine figure of flowing water and crystalline ice, his form constantly shifting between frozen glaciers, crushing ocean depths, and flowing streams, with memories and knowledge frozen within his icy coils. His domain encompasses memory preservation through ice, the crushing power of deep waters, magical energy channeled through frozen currents, and the understanding that some things must be kept frozen to be preserved. He teaches that memory can be frozen in time like ice, that the deepest waters hold the greatest pressure, and that true preservation requires the courage to embrace the cold depths. **Inspired by Jörmungandr, the Norse World Serpent who encircles Midgard in the ocean.**

**Anubiseth, the Shadow Judge (Position 6 - Magenta Shadow)**
The sovereign deity of afterlife guidance and shadow wisdom, Anubiseth serves as the divine judge who guides souls through the mysteries of death, transformation, and rebirth. As the Shadow Judge, she embodies the necessary darkness that balances light, the chaos that enables change, and the wisdom that can only be found by confronting the unknown. Anubiseth appears as a regal figure with the head of a jackal, wreathed in shifting shadows and purple flames, her eyes seeing through all deceptions to the truth beneath. Her domain covers death transitions, shadow magic, beneficial chaos, transformation through crisis, and the wisdom that comes from accepting the unknown. She teaches that shadows are not evil but necessary, that chaos is the engine of growth, and that true wisdom requires the courage to face what lies beyond the light. **Inspired by Anubis, the Egyptian jackal-headed god of the afterlife and mummification.**

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
- **Constitution (Marsalis)**: "Disciplined Might" - physical conditioning and martial endurance
- **Wisdom (Zeusara)**: "Divine Authority, Celestial Justice" - divine wisdom for healing and protection
- **Charisma (Anubiseth)**: "Shadow Wisdom, Underworld Order" - charismatic influence spreads change

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
- **Position 1 (Fire/Surturon)**: Health represents the vital flame that burns in all living things
- **Position 3 (Air/Fenrion)**: Stamina channels wind energy for movement and the endless hunt  
- **Position 5 (Water/Jormunion)**: Mana flows like frozen streams through crystalline memory

**Armor Type Alignment:** Only bridge positions (2, 4, 6) have armor types - Sovereign god alignment.
- **Position 2 (Metal/Marsalis)**: Armor provides disciplined protection through metallic defense
- **Position 4 (Lightning/Zeusara)**: Energy Shield channels divine authority into protective barriers
- **Position 6 (Shadow/Anubiseth)**: Evasion uses shadow wisdom to avoid harm through movement

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
- **Position numbering**: Always 1-6, clockwise from top
- **RGB anchor system**: 1=Red🔴, 3=Green🟢, 5=Blue🔵 are primary anchors
- **Bridge positions**: 2=Yellow🟡, 4=Cyan🔵, 6=Magenta🟣 bridge between RGB anchors
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
| 1 | **RED** 🔴 | Surturon | Strength & Destruction | Health Points, Fire Damage |
| 3 | **GREEN** 🟢 | Fenrion | Dexterity & Hunger | Stamina Points, Air Damage |
| 5 | **BLUE** 🔵 | Jormunion | Intelligence & Preservation | Mana Points, Water Damage |

### Bridge Positions (Sovereign Gods)
These three positions create smooth transitions between the RGB anchors:

| Position | Color | God | Bridge Function | Systems Anchored |
|----------|-------|-----|-----------------|------------------|
| 2 | **YELLOW** 🟡 | Marsalis | Red→Green Bridge | Armor, Metal Damage |
| 4 | **CYAN** 🔵 | Zeusara | Green→Blue Bridge | Energy Shield, Lightning Damage |
| 6 | **MAGENTA** 🟣 | Anubiseth | Blue→Red Bridge | Evasion, Shadow Damage |

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
