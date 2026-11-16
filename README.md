<p align="center"><img src="assets/brand.svg" width="96" alt="EGS-BBS"></p>
<h1 align="center">EGS-BBS</h1>
<p align="center">Empyrion Galactic Survival: Build &amp; Blueprint Ships</p>

[Русский](README.ru.md) · [Release notes](CHANGELOG.md)

A local 3D ship planner for Empyrion and Reforged Eden 2. This repository contains ready-to-run Windows builds and documentation. Development sources are private.

## Download for Windows

**[0.6.0-beta.2 · Windows x64](https://github.com/Tefoke1/EGS-BBS/releases/tag/v0.6.0-beta.2)** — portable ZIP. This is a preview release, not a stable version.

1. Download the ZIP and extract the **entire folder**.
2. Run `EGS-BBS.exe`. No separate Node.js or Python installation is needed.
3. Enter your Steam or SteamLibrary folder. Install Empyrion and subscribe to Reforged Eden 2 beforehand.
4. Wait for the first local model import, then open a downloaded Workshop blueprint from Library.

Keep the EXE together with its adjacent files. Updates use a new extracted folder; local data is stored in `%APPDATA%/EGS-BBS`. Back up your ship as `.ship.json` before updating. The build is not code signed. SHA-256 checksums accompany each release.

## Performance checks

On the test PC, complete first import improved from 8:22 to 3:37 with a 1.04 GB importer peak. All 18,526 output files matched the sequential importer byte for byte. Alexander (27,100 blocks, 4,073,206 triangles) peaked at 2.49 GB working set / 3.51 GB private bytes across the app process group. These are measured results for that workload, not universal guarantees. Subsequent launches reuse cached assets.

## Build and inspect

- Native game models, colors, textures and decals; up to 300,000 blocks.
- Shape catalog with separate material selection. Right-click a placed structural block to replace its material and recalculate mass.
- XYZ sections, category filters, fast/realistic rendering, independent grid and field of view.
- Bottom-to-top, block-by-block timeline and MP4 recording.
- Steam library filters, local autosave, ship component summaries and construction exports.
- Russian and English interface; click the version to read changes.

| Action | Key |
|---|---|
| Select / build / delete tool | V / B / E |
| Delete selection | Del |
| Paint / sample | P / I |
| Rotate 90° / symmetry | R / M |
| Copy / place copy | Ctrl+C / Ctrl+V |
| Undo / redo | Ctrl+Z / Shift+Z (also Ctrl+Shift+Z) |
| Fly / release mouse | F / F or Esc |
| Flight movement / height / boost | WASD / Q,E / Shift |
| Fit ship / hide sidebars | Home / Tab |

Right-click opens block/material options; with the brush it opens the palette. Drag the right mouse button to orbit. Rotation rings turn by 90°; Shift reverses direction.

## Scope and known limits

Workshop `.epb` files can be imported; edited projects are saved as `.ship.json`. **Exporting an edited `.epb` is not supported.** Use the construction plan to build in the game. Mass and power are configuration totals; cargo, fuel, shape adjustments, flight performance and airtightness need in-game verification. Special shaders and effects can differ from the game. Steam subscription dates appear only when Steam stores them explicitly.

Large-ship edits and layer filters update without rebuilding the entire ship. Geometry retains full detail, including nearby devices; automatic distant-device LOD is not included. Initial import and first shader preparation still take time. Long sessions with many individually edited parts can increase draw calls. Native mouse capture and clipboard shortcut checks remain part of beta feedback; browser hosts may prohibit capture.

## Your files and AI

Models and textures are read from your own game installation and are not included in downloads. Original Workshop files are preserved. AI generation is optional and runs only when requested through a detected, signed-in Codex or Claude Code CLI client; its service receives the prompt and build catalog. Regular ChatGPT/Claude desktop windows do not provide this CLI integration: save a generated `.ship.json` from the chat and open it manually.

Unofficial community tool, not affiliated with Eleon Game Studios or the RE2 creators. Game content belongs to its creators. Bundled dependency licenses remain with their runtimes and in `resources/app/dist/vendor`.
