# How EGS-BBS works / Как устроена EGS-BBS

## English

EGS-BBS runs locally on Windows. Electron 45.3.3 hosts the editor, three.js r170 renders ships and bundled Python 3.13 with UnityPy reads assets from the installed game. Models and textures are cached on the PC. The editor reads native `.epb` files, saves personal blueprints and exports PNG or MP4. Editing a Workshop subscription creates a working copy.

The editor talks to a local service on `127.0.0.1`. Its renderer uses context isolation and a sandbox. The desktop bridge opens the folder picker, saves an EPB to a user-selected location and releases temporary import memory. Regular editing stays on the PC. If you choose AI generation, the selected CLI provider receives the prompt and build catalog.

Download the ZIP and `SHA256SUMS.txt` from the same release. Run `Get-FileHash .\EGS-BBS-0.7.0-windows-x64.zip -Algorithm SHA256` in PowerShell and compare the full hash. The EXE is unsigned. The release report lists the checks performed and VirusTotal lookup links. [Release and checks](https://github.com/Tefoke1/EGS-BBS/releases/tag/v0.7.0)

## Русский

EGS-BBS работает локально в Windows. Интерфейс построен на Electron 45.3.3, корабли отображаются через three.js r170. Встроенный Python 3.13 с UnityPy читает ресурсы установленной игры и сохраняет модели и текстуры в кэше на ПК. Редактор открывает игровые `.epb`, сохраняет личные чертежи и экспортирует PNG и MP4. Правки подписок Workshop вносятся в рабочую копию.

Редактор связывается с локальной службой по адресу `127.0.0.1`. Включены изоляция контекста и песочница. Настольный интерфейс предоставляет выбор папки, сохранение EPB по указанному пользователем пути и освобождение временной памяти после импорта. Обычное редактирование выполняется на ПК. При выборе генерации через ИИ запрос и каталог блоков передаются выбранному CLI-провайдеру.

Скачайте ZIP и `SHA256SUMS.txt` из одного выпуска. Команда PowerShell выше вычислит SHA-256 архива. Сравните его целиком со значением в файле. EXE без цифровой подписи. В отчёте выпуска перечислены проведённые проверки и ссылки для поиска по хэшу в VirusTotal. [Выпуск и результаты проверок](https://github.com/Tefoke1/EGS-BBS/releases/tag/v0.7.0)
