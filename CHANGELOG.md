# Changelog

## 0.7.0-beta.10 · 2026-11-19

Empyrion Galactic Survival **1.20.1 (build 5232)** · Reforged Eden 2.

- Models and photo materials took 25.85 and 30.92 seconds to prepare in two empty-cache runs. Beta.9 logged 71.96 seconds on the same PC. Lossless storage reduced the native texture cache from 3.75 to 1.25 GB.
- First launch opens with language selection, then finds Steam libraries. Welcome includes a performance check for all three rendering modes.
- Large projects show loading progress and can be cancelled before the scene changes. Fixed Mantar Dreadnought and Stargate SGU Destiny imports and the incorrect 256-cell export limit.
- Open and save projects in the native EPB format. Saving to the game creates a personal blueprint with a ship portrait. A companion JPG is available for local saves.
- Updated base-game and RE2 catalogs, xeno steel selection and core-based placement. Device groups, transmitters, receivers and 13 circuit types persist in the blueprint.
- The dedicated MP4 workspace combines X/Y/Z layer animation with manual, orbit and cinematic camera paths.

## 0.7.0-beta.1 — 2026-11-17

**Game version:** Empyrion Galactic Survival **1.20.1 (build 5232)** · Reforged Eden 2.

Native EPB export and personal library; million-block capacity and lower large-city memory; cinematic photo/PNG mode; MP4 camera paths, orbit and shot sequence; visible project loading; flight wheel speed; library refresh and material/forcefield fixes. New bilingual illustrated documentation and transparent security notes. Experimental beta: see README for measured limits.

## 0.6.0-beta.2 · 2026-11-16

- Streaming game-archive import: measured peak memory reduced from 7.8 to 1.04 GB without changing models or textures.
- Visible floor-grid switch; grid stays above the floor in realistic mode too.
- Open a saved project on EXE launch using --project.
- First import measured about2.3x faster on the test PC; model/texture counts and elapsed time are visible.
- Ships above10,000 blocks share geometry; painted faces batch independently without losing detail.

## 0.6.0-beta.1 · 2026-11-16

- Native shape catalog and separate material selection.
- Block selection, attached rotation rings and copying.
- Library filters, three-axis sections and inspector tabs.
- New viewport navigation and EGS-BBS branding.
- Large ships: incremental block edits, GPU sections and delta autosaves.
- Replace placed materials with mass recalculation; Ctrl+Z undo and Shift+Z redo.
- Red delete preview, Del for selected parts and visible shortcut labels.
- Large-project outlines, captured flight mouse and first-run Steam setup.

## 0.5.0 · 2026-11-16

- 300,000-block limit, block-by-block construction and MP4.
- Face painting, textures and decals.
- Corrected default material colors and opaque window frames.
