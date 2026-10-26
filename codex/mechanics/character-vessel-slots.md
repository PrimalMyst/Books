# Character Vessel Slot Mechanics

## Concept Metadata
- Concept ID: CONCEPT-VESSEL-SLOTS
- Owner Layer: mechanics
- Related Files:
  - ../diegetic-framing/vessel-acquisition-and-attunement.md
  - ./league-system.md
  - ../lore/myrielle-the-hidden.md
- Status: draft

## Scope
This file defines account-level rules for vessel creation, slot limits, and active-vessel constraints.

## Core Rules
- Max vessels per account per active season: 6.
- Exactly one vessel may be active at a time.
- Player may switch active vessel freely.
- Active vessel is the only vessel that can be directly controlled and receive real-time character progression updates.

## Slot Lifecycle
1. Create vessel: allowed if seasonal slot count is below 6.
2. Activate vessel: sets current vessel context for gameplay session.
3. Deactivate/switch vessel: allowed at player discretion.
4. Migrate vessel: follows season migration rules in ./league-system.md.

## Control Constraint
- Multi-control is not allowed: one player controls one active vessel at a time.
- Non-active vessels cannot be controlled concurrently.

## Progression Scope

### Account-Wide Within a Season
- Selected achievements (configured as account-wide).
- Selected league/season world events and milestone completions (configured as account-wide).
- Account-level unlock flags explicitly marked shared.
- Common stash is shared by all vessels in the same season realm.
- Hideout state is shared by all vessels in the same season realm.

### Shared System Notes
- Common stash includes account-shared storage tabs for that season realm.
- Hideout includes unlocked decorations, layout state, and crafting station access for that season realm.
- Hideout preserves and renders inactive seasonal vessels as visible in-world presences.
- Inactive vessels shown in the hideout are non-controllable display entities.
- Hideout administration authority is account-bound and available from any active vessel in that season.
- Shared stash/hideout scope does not cross season boundaries unless migration rules explicitly allow it.

### Per-Vessel
- Level and build state.
- Inventory and equipment state.
- Quest and story progression.
- Map/area progression unless specifically marked account-wide by season rules.

## Validation Requirements
- Enforce slot cap at creation time and before persistence commit.
- Enforce single-active-vessel invariant on every session start and switch action.
- Enforce that shared progression flags apply to all vessels in the same season.

## Cross-Layer Reference
For in-world explanation of vessel acquisition and one-vessel focus, see ../diegetic-framing/vessel-acquisition-and-attunement.md.
