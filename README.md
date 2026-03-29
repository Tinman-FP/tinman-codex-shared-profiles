# Tinman Codex Shared Profiles

Curated OrcaSlicer profiles organized by machine family for easier sharing and import.

## Download Packages

The published GitHub repo is organized around machine-ready zip packages so each printer family can be downloaded and shared independently.

- `packages/creality-k2-plus.zip`
- `packages/elegoo-centauri-carbon.zip`
- `packages/qidi-x-plus-4.zip`
- `packages/ratrig-v-core-4-idex.zip`
- `packages/snapmaker-u1.zip`
- `packages/sovol-sv08-max.zip`
- `packages/shared.zip`
- `packages/tinman-codex-orca-profiles-full.zip`

## Included Machines

- `orca/sovol-sv08-max`
- `orca/qidi-x-plus-4`
- `orca/elegoo-centauri-carbon`
- `orca/creality-k2-plus`
- `orca/ratrig-v-core-4-idex`
- `orca/snapmaker-u1`
- `orca/shared` for machine-agnostic or cross-machine presets

Each machine folder is split into:

- `machine`
- `process`
- `filament`

## Folder Summary

| Folder | Machine Files | Process Files | Filament Files |
| --- | ---: | ---: | ---: |
| `creality-k2-plus` | 6 | 13 | 20 |
| `elegoo-centauri-carbon` | 12 | 14 | 23 |
| `qidi-x-plus-4` | 6 | 17 | 20 |
| `ratrig-v-core-4-idex` | 18 | 23 | 21 |
| `snapmaker-u1` | 5 | 45 | 16 |
| `sovol-sv08-max` | 8 | 35 | 21 |
| `shared` | 0 | 18 | 10 |

## What This Repo Contains

- Active Codex/Tinman machine presets
- Active tuned process presets
- Active tuned filament presets
- `.info` sidecar files where OrcaSlicer exported them

Excluded from the share set:

- backup files
- imported scaffolding/junk
- obvious `Copy` duplicates

## Import Notes

These files were exported from a live OrcaSlicer user library. Depending on your Orca version and current preset graph, some presets may import as new variants rather than replacing an existing preset.

Best practice:

1. Back up your current Orca user presets first.
2. Import only the machine family you want.
3. Then import the matching process and filament presets.
4. Verify nozzle size, temperatures, acceleration, and chamber assumptions before printing.

## Credits

- William "Tinman" Tinney for profile development, machine tuning direction, print validation, and machine-specific refinement
- OpenAI Codex for preset packaging, organization, cleanup, documentation, and repo preparation

## Notes

- These are practical working presets, not vendor-certified defaults.
- Some folders intentionally keep multiple active generations where they were still present in the live library, such as the Centauri `Codex Tinman` and `Codex Tinman 2` machine variants.
- The `shared` folder exists for presets that are not cleanly tied to one machine by filename alone.
