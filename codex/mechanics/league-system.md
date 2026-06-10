# League System Mechanics

## Concept Metadata
- Concept ID: CONCEPT-SEASONS-LEAGUES
- Owner Layer: mechanics
- Related Files:
	- ../diegetic-framing/seasonal-world-reset.md
	- ../lore/reality-instances.md
	- ../lore/valhalla.md

## Scope
This file defines system behavior for seasons. Narrative meaning is documented in the paired diegetic framing file.

## Realm Types

### Current Season Realities
- Timeboxed cycle (target cadence: 3-4 months).
- Fresh-start character and economy environment.
- Seasonal modifier package enabled for the cycle.
- Competitive progression and event tracking enabled.
- Two flags partition the season into four concurrent realities:
	- default
	- hardcore
	- solo self found
	- hardcore solo self found
- Hardcore: character death is permanent.
- Solo self found: trading with other players is disabled.

### Permanent Realm (Valhalla)
- Persistent progression space across all seasons.
- Receives migrated characters from completed/expired current seasons.
- No full reset of character progression.
- Long-term progression and legacy access live here.

## Season Lifecycle
1. Pre-launch: ruleset and seasonal modifier package are published.
2. Launch: all active-season participants start from clean state.
3. Mid-season: progression, events, and economy run under season rules for each concurrent reality.
4. End-window: final progression window before closure.
5. Closure: active season closes and migration jobs execute.

## Migration Rules

### Triggers
1. Completion trigger: character meets defined completion condition.
2. End-of-season trigger: active season expires.
3. Manual trigger: optional path for eligible offline characters.

### Transfers
- Character level/state.
- Skills and core progression.
- Equipment and inventory (unless season rule marks item class as temporary).
- Completed quest/story flags.
- Account achievements.

### Non-Transfers
- Season-only currencies.
- Season-only temporary modifiers.
- Season ladder rank placement.
- Partial run state (in-progress instance/raid state).

## Character Rules (Per Current Season Reality)
- Max characters per account in one current season reality: 6.
- Only one character can be active at any given moment.
- Player can switch active character freely.
- One player cannot control multiple characters at the same time.
- Progression is mixed: some achievements/world events are account-wide per current season reality, while others are per character.
- Common stash and hideout are account-shared across all characters in the same current season reality.
- New character creation is blocked when the current season reality character cap is reached.

For full slot/attunement rules and edge cases, see ./character-vessel-slots.md.
For in-world explanation, see ../diegetic-framing/vessel-acquisition-and-attunement.md.

## Reset Boundaries
- Active season reset affects active-season-only state.
- Eternal realms are not hard-reset by season turnover.
- Historical season data is archived for audit and records.

## Validation Requirements
- Each season must define transfer whitelist/blacklist before launch.
- End-of-season migration must be idempotent and retry-safe.
- Player-visible migration results must be auditable.

## Cross-Layer Reference
For in-world explanation of why resets and migrations happen, see ../diegetic-framing/seasonal-world-reset.md.



