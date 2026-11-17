<p align="center"><img src="assets/brand.svg" width="80" alt="EGS-BBS"></p>
<h1 align="center">EGS-BBS</h1>
<p align="center">Empyrion Galactic Survival: Build &amp; Blueprint Ships</p>
<p align="center">
  <a href="https://github.com/Tefoke1/EGS-BBS/releases/tag/v0.7.0-beta.1"><img src="assets/navigation/app.svg" height="44" alt="EGS-BBS 0.7.0-beta.1"></a>
  <a href="https://store.steampowered.com/news/app/383120"><img src="assets/navigation/game.svg" height="44" alt="Empyrion 1.20.1 · 5232"></a>
  <a href="CHANGELOG.ru.md"><img src="assets/navigation/active-ru.svg" height="44" alt="Активная разработка"></a>
</p>
<p align="center">
  <a href="README.md"><img src="assets/navigation/language-ru.svg" height="44" alt="English"></a>
  <a href="https://github.com/Tefoke1/EGS-BBS/releases/tag/v0.7.0-beta.1"><img src="assets/navigation/download-ru.svg" height="44" alt="Скачать"></a>
  <a href="CHANGELOG.ru.md"><img src="assets/navigation/notes-ru.svg" height="44" alt="Что нового"></a>
  <a href="docs/TRUST.md"><img src="assets/navigation/architecture-ru.svg" height="44" alt="Как устроено"></a>
  <a href="docs/DEPENDENCIES.md"><img src="assets/navigation/licenses-ru.svg" height="44" alt="Лицензии"></a>
  <a href="#системные-требования"><img src="assets/navigation/hardware-ru.svg" height="44" alt="Требования к ПК"></a>
  <a href="#карта-разработки"><img src="assets/navigation/roadmap-ru.svg" height="44" alt="Карта разработки"></a>
</p>

EGS-BBS — локальный конструктор чертежей для Empyrion и Reforged Eden 2: просмотр по слоям, планирование постройки и редактирование кораблей из игры и Workshop.

![Конструктор EGS-BBS: Thanatos](assets/showcase-full.png)

## Системные требования

| Компонент | Рекомендуется |
|---|---|
| ОС | Windows 11 x64 |
| Процессор | Многоядерный x64; проверен AMD Ryzen 7 5700X3D |
| ОЗУ | 16 ГБ для обычных кораблей; 32 ГБ для крупных проектов |
| Видеокарта | Аппаратный WebGL 2; для крупных проектов и фоторежима — 8 ГБ видеопамяти. Проверена Radeon RX 5700 XT |
| Диск | SSD, несколько свободных ГБ под приложение и кэш; отдельно — место под игру и чертежи |
| Игра | Установленная Empyrion; скачанный Reforged Eden 2 для его блоков |

## Послойный просмотр

Выбирайте диапазон по X, Y или Z либо один слой, чтобы рассмотреть внутренние помещения и расположение устройств.

| X · поперёк корпуса | Y · по палубам | Z · вдоль корабля |
|:---:|:---:|:---:|
| ![Слои X](assets/layers-x.gif) | ![Слои Y](assets/layers-y.gif) | ![Слои Z](assets/layers-z.gif) |

## Устройства крупным планом

Скрывайте корпус, оружие и двигатели независимо друг от друга. Приближайте камеру к деталям или перемещайтесь в режиме полёта.

![Переключение корпуса, оружия и двигателей с приближением камеры](assets/components-camera.gif)

## Конструирование

- Игровые формы, материалы, окраска и декали.
- Выбор, копирование, поворот на 90°, симметрия, отмена и повтор действий.
- Состав корабля, масса, мощность, CPU и оценка ресурсов фабрики.
- Таймлайн постройки снизу вверх, блок за блоком.
- Проекты до 1 000 000 блоков; сохранение работы в `.ship.json`.
- Быстрый, реалистичный и экспериментальный кинематографичный режимы.

## Из чертежа — в игру

1. Откройте личный чертёж или подписку Workshop из **Библиотеки** и внесите изменения.
2. Нажмите **«В игру»**: новый `.epb` сохранится в личную папку чертежей Empyrion.
3. В игре отправьте чертёж на фабрику, внесите требуемые ресурсы и после производства разместите корабль.

Итоговые ресурсы и ограничения постройки определяет игра. Порядок публикации в Workshop доступен в окне экспорта.

## Фото и видео

Настраивайте свет и экспозицию, сохраняйте PNG до 4K или MP4. Для съёмки доступны плавная ручная камера, облёт по орбите и смена ракурсов.

![YAMATO Real Size: экспорт PNG из EGS-BBS](assets/photo-yamato.png)

<details>
<summary>Настройки съёмки</summary>

![Настройки кадра и камеры](assets/filming.png)

</details>

## Запуск и обновление

1. Скачайте ZIP по кнопке **«Скачать»** и распакуйте его целиком.
2. Запустите `EGS-BBS.exe` — отдельная установка Python и Node.js не нужна.
3. Укажите папку Steam / SteamLibrary и дождитесь импорта игровых ресурсов. Следующие запуски используют кэш.

Для обновления распакуйте новую версию отдельно, предварительно сохранив проекты в `.ship.json`. Данные приложения находятся в `%APPDATA%/EGS-BBS`.

В выпуске приложены `SHA256SUMS.txt` и `SECURITY-REPORT.md`. Текущая бета — без цифровой подписи.

<details>
<summary>Горячие клавиши</summary>

| Действие | Клавиша |
|---|---|
| Выбрать / строить / удалять | V / B / E |
| Удалить выбранное / кисть / пипетка | Del / P / I |
| Поворот / симметрия | R / M |
| Копировать / вставить / отменить / повторить | Ctrl+C / Ctrl+V / Ctrl+Z / Shift+Z |
| Полёт / выход | F / F или Esc |
| Перемещение / высота | WASD / Q,E |
| Скорость полёта | Колесо; Shift ×4; Ctrl+Shift ×16; Alt ×¼ |
| Вписать корабль / скрыть панели | Home / Tab |

Правая кнопка — меню блока и материалов; при покраске — палитра.

</details>

## Карта разработки

![Планы: расчёт тяги и перегрузки; герметичность и центр масс; строительство; ИИ; сигналы и логика; оптимизация; видео; исправления по сообщениям сообщества](assets/roadmap-ru.svg)

## Поддержать разработку

Если вам понравилась работа и хочется поучаствовать в развитии EGS-BBS, меня можно поддержать на Boosty.

<a href="https://boosty.to/alienlorem"><img src="assets/boosty-ru.svg" width="270" alt="Поддержать на Boosty"></a>

## Авторы и благодарности

Приложение использует ресурсы локально установленной игры. Модели и текстуры принадлежат [Eleon Game Studios](http://www.eleon-studios.com) и авторам контента; в дистрибутив они не входят.

В вышеуказанных снимках, демонстрирующих возможности программы, использованы работы авторов:

- MisterCrow — ["Thanatos" Assault Vessel](https://steamcommunity.com/sharedfiles/filedetails/?id=1090967294)
- MISOsp[HZ_Express] — [YAMATO Real Size](https://steamcommunity.com/sharedfiles/filedetails/?id=1320029358)

[Сообщить о проблеме](https://github.com/Tefoke1/EGS-BBS/issues)
