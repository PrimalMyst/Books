# Divine Influence System - Updated Framework

## Summary of Changes

The divine influence system has been completely revised to clarify the fundamental differences between humanoids and monsters, while removing racial restrictions on divine followings.

## Core Principles Established

### **1. Divine Influences Are Not Race-Specific**
- **Old System**: Races had predefined divine affinities (e.g., Canine Beast Folk → Korthak, Aurelius, Voltharion)
- **New System**: Any playable race can follow any combination of gods
- **Key Change**: Divine capacity defines humanoid heritage, not which specific gods are followed

### **2. Humanoid Divine Requirements**
- **Minimum for Significance**: All heroes, leaders, and world-changing figures must have at least one influence from each accessible divine tier:
  - **Fundamental Gods**: Pyrion (Fire), Glacius (Cold), or Voltharion (Lightning)
  - **Primal Gods**: Serafina (Chaos), Aurelius (Radiance), or Korthak (Physical)
- **Myrielle's Limitation**: "The Hidden" cannot directly influence humanoids - she works through monster companions and mounts
- **Transcendent Potential**: Advanced humanoids can channel multiple influences from the accessible tiers

### **3. Monster Divine Limitations**
- **Universal Limitation**: All monsters limited to maximum 2 divine influences
- **Special Cases**: Mounts and monster companions must include Myrielle + one other god
- **No Exceptions**: Even legendary monsters cannot exceed the 2-influence limit

## Schema Updates

### **Character Schema Changes**
```json
"divine_influences": {
  "fundamental_gods": ["pyrion", "glacius", "voltharion"],
  "primal_gods": ["serafina", "aurelius", "korthak"],
  "myrielle_guidance": {
    "direct_influence": false,
    "indirect_support": "description of companion/mount support"
  }
}
```
- Enforces accessible tier requirement for significant characters
- Prevents direct Myrielle influence on humanoids
- Tracks indirect support through companions/mounts

### **Monster Schema Changes**
```json
"divine_influences": {
  "influences": ["god1", "god2"],
  "myrielle_requirement": true/false
}
```
- Maximum 2 influences enforced
- Myrielle requirement flag for mounts/companions
- Clear cosmic limitation tracking

## Example Updates

### **Character Example**
- **Astrid the Mist-Walker**: Now has Voltharion (Fundamental), Aurelius (Primal), with Myrielle support through companions
- Demonstrates accessible tier requirement while showing Myrielle's indirect influence

### **Mount Example** 
- **Stormwing Eagle**: Now has Myrielle (bonding) + Voltharion (storm powers)
- Shows Myrielle requirement for mystical mount bonding

### **Companion Example**
- **Silverlight Wisp**: Now has Myrielle (guidance) + Aurelius (light/navigation)
- Demonstrates guidance channeling through Myrielle

### **Standard Monster Example**
- **Shadowmane Stalker**: Has Serafina (shadow) + Korthak (hunt)
- Shows standard 2-influence limit without Myrielle

## Documentation Updates

### **Playable Races (playable-races.md)**
- Removed race-specific divine affinities
- Added trio requirement explanation
- Emphasized race independence from divine choices
- Clarified Myrielle requirement for mounts/companions

### **Monster Classification (monster-classification-lore.md)**
- Updated companion sections with Myrielle requirement
- Added symbiotic relationship explanations
- Clarified combat limitations for monster companions

### **Lore Data (humanoid-legacy.json)**
- Removed racial divine affinities
- Added trio requirement explanations
- Updated mount/companion divine patterns
- Fixed JSON structure issues

## Key Benefits of New System

### **1. Clearer Distinctions**
- Humanoids: Multi-tier divine capacity from 6 accessible gods (Fundamental + Primal)
- Monsters: Maximum 2 influences total
- Mounts/Companions: Myrielle + 1 other (special case within 2-limit)
- Myrielle: Can only influence through monsters, not humanoids directly

### **2. Character Freedom**
- Players can choose any divine combination regardless of race
- Race provides physical traits, not spiritual limitations
- Divine choices reflect character development, not racial stereotypes

### **3. Lore Consistency**
- Explains mount burden-sharing through Myrielle's bonding influence
- Justifies companion guidance through Myrielle's wisdom fragments
- Maintains cosmic law separation between humanoids and monsters

### **4. Gameplay Integration**
- Mount system: Mystical burden-sharing explains inventory mechanics
- Companion system: Guidance abilities explain HUD enhancements
- Social dynamics: Divine capacity determines natural hierarchy

## Implementation Status

✅ **Schema Files**: Updated to enforce new rules  
✅ **Example Files**: All examples updated to new structure  
✅ **Documentation**: Comprehensive updates across all codex files  
✅ **Lore Consistency**: All divine references use new system  
✅ **JSON Validation**: All files pass schema validation

The divine influence system now provides clear, consistent rules that enhance both lore depth and gameplay mechanics while maintaining the fundamental distinction between humanoids and monsters based on cosmic law rather than arbitrary limitations.
