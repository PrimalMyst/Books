# Gear - Customizable Equipment

High-end equipment that can be extensively modified, enhanced, and personalized through various systems.

## Hexagon Alignment per Folder
- armors/ — aligned by armor type: Armor (AR), Energy Shield (ES), Evasion (EV), plus their hybrids (AR+ES, AR+EV, ES+EV)
- accessories/ — aligned by resources: Health, Mana, Stamina
- weapons/ — aligned by schools with color mapping:
  - martial = red
  - ballistic = green
  - arcane = blue
  - Note: each weapon item also has an element layer (all 6 corners): fire, metal, air, lightning, water, shadow

## Categories

### `accessories/`
- Wearable bonuses: rings, amulets, earrings, belt locks
- Alignment: Resource-based (Health, Mana, Stamina)
- Features: Enchantments, gem socketing, divine resonance tuning
- Variations: Unique legendary versions with special lore and abilities
- Enhancement: Upgradeable through divine trials, crafting, and achievements

### `armors/`
- Protective equipment aligned to 3 sovereign armor types (and hybrids)
  - Armor (Physical protection)
  - Energy Shield (Magical barriers)
  - Evasion (Movement-based defense)
  - Hybrids: AR+ES, AR+EV, ES+EV
- Features: Material upgrades, enchantments, appearance modifications
- Variations: Set pieces, legendary variants, god-specific designs
- Enhancement: Defense scaling, resistance improvements, visual effects

### `weapons/`
- Combat equipment organized by school → hand-category → type
  - Schools (color-aligned): martial (red), ballistic (green), arcane (blue)
  - Hand-categories: two_handed, one_handed, addons
  - Types: e.g., swords (longswords, shortswords), maces (heavy-maces, maces), bows, staves, wands, shields, etc.
  - Element: per-item attribute from the 6-corner set: fire, metal, air, lightning, water, shadow
- Features: Damage type conversion, ability modifications, appearance customization
- Variations: Legendary weapons with unique abilities and rich lore
- Enhancement: Damage scaling, elemental infusions, combat style adaptation

## Design Philosophy
All gear participates in the hexagonal design for balanced progression and thematic consistency:
- Armors: AR/ES/EV (and hybrids) determine defensive identity
- Accessories: Resource alignment (Health/Mana/Stamina) guides utility
- Weapons: School color alignment defines style; element per-item adds the 6-corner layer for damage/affinity
