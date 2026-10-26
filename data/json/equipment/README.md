# Equipment System - Dual Category Structure

Equipment organized into two main categories based on customization capabilities and mechanical complexity.

## Structure

### `gear/` - Customizable Equipment
High-end items that can be extensively modified and enhanced:
- `accessories/` - Rings, amulets, jewelry (enchantments, socketing, divine tuning)
- `armor/` - Protective equipment (upgrades, modifications, set pieces)
- `weapons/` - Combat gear (damage conversion, ability mods, hexagonal alignment)

### `items/` - Fixed Utility Equipment  
Standardized items with consistent properties:
- `consumables/` - Potions, scrolls, buffs (single-use, fixed effects)
- `materials/` - Crafting components, resources, recipes (standard quantities)
- `cosmetics/` - Capes, veils, masks (visual only, no mechanical benefits)

## Design Philosophy

**Gear**: Complex equipment that grows with the player through hexagonal system integration. Supports deep customization, enhancement systems, and legendary variations aligned with the 6-position hexagonal layout.

**Items**: Utility and cosmetic items with reliable, predictable effects. Supports game economy balance, visual personalization, and future combination/collection systems.

## Hexagonal Integration
Gear follows the 6-position hexagonal system:
1. **Red** (Strength) - Staves/Wands | 2. **Yellow** (Constitution) - Daggers/Orbs
3. **Green** (Dexterity) - Bows/Javelins | 4. **Cyan** (Wisdom) - Swords/Axes  
5. **Blue** (Intelligence) - Hammers/Mauls | 6. **Magenta** (Charisma) - Shields/Maces

## Reference
See: `HEXAGONAL_SYSTEMS_MAPPING_DRAFT.md` - Equipment Types section
