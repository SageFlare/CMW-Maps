# CMW-Maps

Chivalry: Medieval Warfare maps rebuilt for Chivalry 2 Unchained, as free-for-all maps.

**Dev/test build (0.x), not a public release.** Shared with the Unchained developers for testing, including mod-loading time. The maps are converted from the original CMW map data by an automated pipeline (same layout, scale, lighting, sounds and effects where the conversion supports them), then checked in game. Expect rough edges.

## Maps

| Map | Type in CMW | PAK | Map name |
|---|---|---|---|
| Cistern | Duel | `CMW_Cistern.pak` | `FFA_CMW_Cistern` |
| Courtyard | Duel | `CMW_Courtyard.pak` | `FFA_CMW_Courtyard` |
| Frost Peak | Duel | `CMW_FrostPeak.pak` | `FFA_CMW_FrostPeak` |
| Arena | Duel | `CMW_Arena.pak` | `FFA_CMW_Arena` |
| Coldfront | Team objective | `CMW_Coldfront.pak` | `FFA_CMW_Coldfront` |
| Battlegrounds | Team objective | `CMW_Battlegrounds_v3.pak` | `FFA_CMW_Battlegrounds_v3` |
| Outpost | Team objective | `CMW_Outpost.pak` | `FFA_CMW_Outpost` |

All maps play as free-for-all. The CMW objective and duel modes are not ported.

## Installation

1. Download [`CMW_Library.pak`](https://github.com/SageFlare/CMW-Library/releases/latest). Every map needs it.
2. Download the map PAKs you want from the [latest release](https://github.com/SageFlare/CMW-Maps/releases/latest). Each map is its own PAK; install only the ones you play.
3. Copy them into `Chivalry 2/TBL/Content/Paks/`.
4. Launch through the [Unchained Launcher](https://github.com/Chiv2-Community/UnchainedLauncher).
5. Load a map from the console, e.g. `open /Game/Mods/AgMods/CMW_AOCDuel-Cistern/FFA_CMW_Cistern`. The path pattern is `/Game/Mods/AgMods/<folder>/<map name>`, with these folders: `CMW_AOCDuel-Cistern`, `CMW_AOCDuel-Courtyard`, `CMW_AOCDuel-FrostPeak`, `CMW_AOCDuel-Arena`, `CMW_AOCTO-Coldfront`, `CMW_AOCTO-Battlegrounds_v3`, `CMW_AOCTO-Outpost`.

Each release lists every PAK's SHA256 (`<name>.pak.sha256`).

## Known issues

- **Delay after loading:** about 30 s after a map loads, Unchained's mod loader runs its asset scan over all installed mods. The time grows with the number of installed mod packages. The Unchained developers are looking at it.
- **Not ported yet:** CMW fog and bloom (the maps can look clearer and flatter than in CMW), moving and tiled decals, some sound shapes, and CMW objective/duel logic.
- **Coldfront:** some smoke and cloud effects show dark squares (under investigation). One-shot debris effects start switched off on Coldfront, because placed debris effects that run at load crashed the game about 50 s later.

## Credits

- Original maps: Chivalry: Medieval Warfare by Torn Banner Studios.
- Port: SageFlare.
- Modding toolchain: the Chivalry 2 Unchained community (Unchained Launcher, ArgonSDK).

The conversion scripts are not public yet.

See [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) for what the license covers.
