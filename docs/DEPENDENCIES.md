# Third-party software / Сторонние компоненты

The application is not offered under an open-source license. Development sources remain private. Third-party components retain their own licenses and notices; this does not transfer rights to game content. / Исходники приложения закрыты. Лицензии библиотек сохраняются и не предоставляют прав на контент игры.

| Component | Version | Purpose | License |
|---|---|---|---|
| Electron | 45.3.3 | Desktop, Chromium, Node.js | MIT; Chromium and bundled component notices in LICENSES.chromium.html |
| three.js | r170 | WebGL rendering | MIT |
| Mediabunny | 1.66.0 | MP4 encoding/muxing | MPL-2.0 |
| Python | 3.13 | Local importer runtime | PSF-2.0 and bundled notices |
| UnityPy | 1.25.4 | Read installed Unity assets | MIT |
| dnfile | 0.18.0 | Read .NET metadata | MIT |
| dncil | 1.0.2 | Read CIL | Apache-2.0 |
| cryptography | 50.0.2 | Local game format compatibility | Apache-2.0 OR BSD-3-Clause |
| Pillow | 13.0.0 | Image conversion | MIT-CMU |

Mediabunny is bundled from unmodified published source: [version 1.66.0](https://www.npmjs.com/package/mediabunny/v/1.66.0), [upstream](https://github.com/Vanilagy/mediabunny). The bundle, full MPL license and source notice are in resources/app/dist/vendor. Python distribution metadata includes dependency license texts; Electron's LICENSE and LICENSES.chromium.html are retained. The release includes a machine-readable dependency inventory and a collected LICENSES directory. Build-only tools such as esbuild and Electron Packager are not the application runtime.

## Full Python dependency inventory

| Package | Version |
|---|---|
| archspec | 0.2.7 |
| astc-encoder-py | 0.1.12 |
| attrs | 26.1.0 |
| brotli | 1.2.1 |
| cffi | 2.1.1 |
| cryptography | 50.0.2 |
| dncil | 1.0.2 |
| dnfile | 0.18.0 |
| etcpak | 0.9.15 |
| fmod_toolkit | 0.1.3 |
| fsspec | 2026.9.0 |
| lz4 | 4.4.5 |
| pefile | 2024.8.26 |
| pillow | 13.0.0 |
| pycparser | 3.12 |
| pyfmodex | 0.7.2 |
| texture2ddecoder | 1.0.6 |
| tpk_ar | 0.2.4 |
| UnityPy | 1.25.4 |
