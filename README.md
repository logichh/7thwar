# 7th Heaven War

7th Heaven War is a Towny-based war plugin built to replace SiegeWar with a cleaner, controlled, and highly configurable war experience.

## Core Features
- Full war lifecycle: preparation, fighting, break, and treaty phases.
- Banner-based sieges with capture timers, recapture flow, and chunk ownership transfer.
- Diplomacy system with peace, neutrality, and surrender requests that require acceptance.
- Defender counteroffensive mode (retaliation) for higher-risk defensive wars.
- Economy pressure with scheduled war upkeep and surrender penalties.
- Siege-zone combat rules: PvP zones, TNT limits, anti-cheese movement/item restrictions.
- Live siege UI with holograms and boss bars.
- War Command Center menu for Java players and Bedrock forms via Floodgate.
- Discord webhook event feed (declare, start, end, siege events, diplomacy events).
- Persistent state saving and recovery after server restarts.
- Admin control tools for ending wars/sieges, skipping prep, and clearing stuck requests.

## Systems Included
- `War Engine`: phase rotation, war status, diplomacy cooldowns, retaliation toggles.
- `Siege Engine`: banner validation, adjacency checks, capture/recapture logic, claim updates.
- `Economy Engine`: hourly upkeep cycle, defeat by insolvency, war balance persistence.
- `Restriction Engine`: build/PvP/mobility/TNT enforcement around active siege zones.
- `Menu System`: GUI workflows for declare/peace/neutrality/surrender/pending/timers/guide.
- `Persistence Layer`: autosave + restore for wars, sieges, economy timers, neutrality timers.
- `Integration Layer`: Towny core integration, optional Floodgate Bedrock support, Discord alerts.
- `API`: `WarZoneAPI` for checking if a location is near active war activity.

## Commands
- Player: `/war`, `/declare war`, `/peace`, `/neutrality`, `/surrender`, `/wars list`, `/sieges list`
- Admin: `/waradmin list|end|endall|skipprep|clearrequests|endsiege|endallsieges`
