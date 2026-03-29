# Tinman Codex Shared Profiles

Curated OrcaSlicer profiles developed and refined by William "Tinman" Tinney with Codex support, organized by machine family for easy sharing, import, and reuse.

## Quick Start

If you just want the easiest path:

1. Download the zip for your printer from `packages/`.
2. Unzip it locally.
3. In OrcaSlicer, import the matching `machine`, `process`, and `filament` presets.
4. Start with the nozzle size you actually run on that machine.
5. Review temperatures, chamber assumptions, and acceleration before your first print.

If you want everything, use:

- `packages/tinman-codex-orca-profiles-full.zip`

## Download Packages

The repo includes machine-ready zip packages so each printer family can be shared independently.

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

## Start Here

Recommended starting machine presets by family:

- `Sovol SV08 MAX`: start with `Sovol SV08 MAX 0.4/0.6/0.8/1.0 nozzle Codex Tinman`
- `Qidi X-Plus 4`: start with `Qidi X-Plus 4 0.4/0.6/0.8 nozzle - Codex Tinman`
- `Elegoo Centauri Carbon`: start with `Elegoo Centauri Carbon ... - Codex Tinman`; try the `Codex Tinman 2` variant only if you specifically want that newer branch
- `Creality K2 Plus`: start with `Creality K2 Plus 0.4/0.6/0.8 nozzle - Codex Tinman`
- `RatRig V-Core 4 IDEX`: start with the standard `RatRig V-Core 4 IDEX 500 ... - Codex Tinman`; use `COPY MODE` or `MIRROR MODE` only when that workflow is intentional
- `Snapmaker U1`: start with the nozzle-size-matched `Codex Best Quality`, `Codex Fine`, or `Codex Draft` process family after importing the base machine preset

## Recommended First Presets

If you are just getting started, these are the easiest entry points:

| Machine | Common Starting Nozzle | Machine Preset | Process Preset | Notes |
| --- | --- | --- | --- | --- |
| `Sovol SV08 MAX` | `0.6` | `Sovol SV08 MAX 0.6 nozzle Codex Tinman` | `0.24mm Codex Best Quality @Sovol SV08 MAX 0.6 nozzle` | Strong general-purpose starting point for the SV08 MAX family |
| `Qidi X-Plus 4` | `0.6` | `Qidi X-Plus 4 0.6 nozzle - Codex Tinman` | `0.24mm Codex Best Quality @Qidi X-Plus 4 0.6 nozzle` | Good default balance of speed and finish |
| `Elegoo Centauri Carbon` | `0.6` | `Elegoo Centauri Carbon 0.6 nozzle - Codex Tinman` | `0.24mm Codex Best Quality @Elegoo Centauri Carbon 0.6 nozzle` | Try the plain `Codex Tinman` branch first before `Codex Tinman 2` |
| `Creality K2 Plus` | `0.6` | `Creality K2 Plus 0.6 nozzle - Codex Tinman` | `0.24mm Codex Best Quality @Creality K2 Plus 0.6 nozzle` | Best starting point for shared engineering and general printing |
| `RatRig V-Core 4 IDEX` | `0.6` | `RatRig V-Core 4 IDEX 500 0.6 nozzle - Codex Tinman` | Use the nozzle-matched `Codex Best Quality` or `Codex Fine` family in that machine folder | Start with standard mode before trying `COPY MODE` or `MIRROR MODE` |
| `Snapmaker U1` | `0.4` | Start with the base `Snapmaker U1` machine preset you intend to pair with the process family | `0.16mm Codex Best Quality @Snapmaker U1 0.4 nozzle` | Easiest entry point before moving to the larger nozzles and specialty process variants |

If you prefer speed first, look for the `Codex Draft` preset family. If you prefer surface quality first, start with `Codex Best Quality`.

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
- imported scaffolding and junk presets
- obvious `Copy` duplicates that were not part of the intended live library

## Import Notes

These files were exported from a live OrcaSlicer user library. Depending on your Orca version and current preset graph, some presets may import as new variants rather than replacing an existing preset.

Recommended import order:

1. Back up your current Orca user presets first.
2. Import the `machine` presets for the printer family you want.
3. Import the matching `process` presets.
4. Import the matching `filament` presets.
5. Open the chosen printer preset and confirm nozzle size, chamber behavior, max volumetric flow, and acceleration assumptions before printing.

## Versioning

This repo is intended to be shared both as a live library and as stable version snapshots. Tagged versions are useful if you want to point Reddit users or collaborators at a fixed set of files instead of a moving branch tip.

## Credits

- William "Tinman" Tinney for profile development, machine tuning direction, print validation, and machine-specific refinement
- OpenAI Codex for preset packaging, organization, cleanup, documentation, and repo preparation

## Notes

- These are practical working presets, not vendor-certified defaults.
- Some folders intentionally keep multiple active generations where they were still present in the live library, such as the Centauri `Codex Tinman` and `Codex Tinman 2` machine variants.
- The `shared` folder exists for presets that are not cleanly tied to one machine by filename alone.
- Treat these as strong starting points, then fine-tune for your exact machine condition, filament brand, and environment.
