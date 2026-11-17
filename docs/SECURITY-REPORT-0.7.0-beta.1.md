# Release verification — 0.7.0-beta.1

2026-11-17. Windows x64 portable beta. **Unsigned; independent antivirus analysis is pending.** This report does not certify absence of malware.

| File | SHA-256 |
|---|---|
| EGS-BBS-0.7.0-beta.1-windows-x64.zip (190,653,486 bytes) | `4ef2f0c7e86ba3b7d2c66a1d5d95169357dcc53a9de337a0b518c5ce4e36f782` |
| EGS-BBS.exe inside the ZIP | `2bda31ef532dc9cb641d0e9cb7a7247e2937b793789164cb21cd62bfbc431ce5` |

## VirusTotal

**No fresh VirusTotal scan has been completed for this release. Do not interpret the links below as clean scan results.** Submission/analysis is pending; a missing report means no available result.

- [ZIP hash lookup](https://www.virustotal.com/gui/file/4ef2f0c7e86ba3b7d2c66a1d5d95169357dcc53a9de337a0b518c5ce4e36f782)
- [EXE hash lookup](https://www.virustotal.com/gui/file/2bda31ef532dc9cb641d0e9cb7a7247e2937b793789164cb21cd62bfbc431ce5)

Scanning only Electron's EXE does not assess all shipped JavaScript, Python, DLLs and other runtime content. The full ZIP matters. VirusTotal public submission shares the submitted file with its analysis ecosystem; never upload personal projects or private repositories. No Windows Defender scan result is claimed.

## Checks performed

- ZIP CRC verified; uploaded GitHub asset SHA-256 matches the local archive.
- Authenticode: `NotSigned`.
- Artifact inspection covered 1,515 files, including the nested Python ZIP: 460,195,999 uncompressed bytes. Credential signatures, complete private-key blocks, known installed-game secret values in raw/hex/base64/applicable UTF-16 forms, personal-machine paths and sensitive filenames: no matches. This is not an exhaustive code or malware audit.
- Generated Python bytecode containing test-machine paths was removed before archiving. No game model/texture cache, Workshop blueprints, personal saves, AI jobs or developer credentials included.
- 83 JavaScript tests passed. Clean packaged first-run import completed in 283 seconds; 799 locally available ships discovered; YAMATO with 25,440 roots opened in the packaged application server UI. Timing is specific to the test PC.
- Third-party notices, Python distribution license metadata and collected LICENSES included. BUILD.json records the source revision and EXE hash. Development sources remain private; runtime JS/Python is inspectable.

## По-русски

Выпуск не подписан. **Свежий анализ VirusTotal пока не выполнен**; ссылки выше — поиск по точному хэшу, а не доказательство успешной проверки. Результат будет дополнен после анализа. Проверка одного EXE не заменяет проверку всего архива.

Контрольная сумма GitHub совпала с локальным ZIP; CRC проверен. Проверены 1 515 файлов, включая вложенный Python ZIP: секреты по используемым сигнатурам, известные игровые ключи, личные пути и запрещённые имена файлов не найдены. Это не полный аудит вредоносного кода. Первый импорт готовой сборки и открытие корабля проверены, 83 теста прошли. Не отключайте антивирус или SmartScreen; исследуйте предупреждения.
