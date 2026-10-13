# FeralZombie — замена звуков и музыки Vintage Story

> Папка напарницы. Документация по замене **всех звуков и музыки** в игре.
> Версия игры: **v1.21.5**. Все пути относительны к корню папки `Vintage Story v1.21.5/`.

---

## 1. Коротко (TL;DR)

- Все звуки и музыка лежат в папке **`assets/`** игры, в подпапках `sounds/` и `music/` трёх «пакетов» (asset packs):
  - `assets/game/` — базовые звуки/музыка (движок, общий набор).
  - `assets/survival/` — основной контент выживания (звери, блоки, эффекты, основная музыка).
  - `assets/creative/` — немного музыки для творческого режима.
- **Формат: только `.ogg` (Vorbis)** — в этой сборке **688 файлов, все `.ogg`**. Поддерживается также `.wav` (PCM) — движок определяет формат по первым 4 байтам (`RIFF` → WAV, иначе → OGG), но все оригинальные ассеты — OGG.
- Звук в играх ссылают по **относительному пути без расширения**:
  - в JSON блоков/сущностей: `"sounds": { "place": "block/planks", ... }` → ищется `sounds/block/planks.ogg` внутри того же пакета;
  - в `soundconfig.json`: саунд-сеты (`"walk/wood1"` и т.п.);
  - в `musicconfig.json`: треки (`"file": "night-to-day"` → `music/night-to-day.ogg`).
- **Чтобы заменить звук** — положи свой файл с **тем же именем** в **тот же путь** (или поменяй ссылку в JSON/конфиге). См. §4 и §6.

---

## 2. Где лежат файлы (структура)

### 2.1 Музыка

| Путь | Файлов | Что это |
|------|--------|---------|
| `assets/survival/music/` | 41 `.ogg` + `musicconfig.json` | Основная музыка поверхности (day/night/season) + event-треки |
| `assets/survival/music/deepunderground/` | 33 `.ogg` | Фоновая музыка пещер (ambient-слой, `CaveMusicTrack`) |
| `assets/survival/music/tuningcylinder/` | 4 `.ogg` | Треки «резонанса» / тюнинг-цилиндра (event) |
| `assets/game/music/` | 3 `.ogg` + `musicconfig.json` | Базовые треки (night-to-day, nostalgic, roots) |
| `assets/creative/music/` | 3 `.ogg` + `musicconfig.json` | Музыка creative-режима |

**Как подбирается трек** — файл `assets/survival/music/musicconfig.json` (и аналогичные в `game/` и `creative/`). Там список `tracks[]`, каждый с `$type`:
- `SurfaceMusicTrack` — обычный фоновый трек на поверхности. Поля: `file` (имя без `.ogg`), `name`, `onPlayList` (`survival` / `creative`), `minhour`/`maxhour` (часы суток), `minSeason`/`maxSeason`, `minLatitude`/`maxLatitude`, `maxTemperature`, `startPriority`. **Важно: `file` — это путь относительно `music/`, расширение `.ogg` добавляется движком автоматически.**
- `EventMusicTrack` — трек по событию (напр. `schematicCode: "resonancearchive"` → играет при входе в «Архив резонанса»).
- `CaveMusicTrack` — музыка пещер: `parts[]` со списком `files` (паттерны со звёздочкой, напр. `"deepunderground/aquatic drone*"` — любой файл, начинающийся с `aquatic drone`), `stopMusic: true` (останавливает поверхностную музыку), `maxSunlight: 12` (включается, когда свет < 12).

**Правила задержки** (общие для `musicconfig.json`): `properties.mindelay` = 4с, `maxdelay` = 8с — пауза между треками.

### 2.2 Звуки

| Путь | Файлов | Что это |
|------|--------|---------|
| `assets/survival/sounds/block/` | 85 | Звуки блоков: ломать/бить/ставить (дерево, стекло, металл, керамика, двери, ящики, руды) |
| `assets/survival/sounds/block/creak/` | 7 | Скрип дерева/балок |
| `assets/survival/sounds/creature/` | 23 (+ подпапки) | Звуки существ: дрifter, цикада, цоклокур (coqui), кролик и др. |
| `assets/survival/sounds/creature/{bear,chicken,goat,...}/` | — | Звуки конкретных животных (по подпапкам) |
| `assets/survival/sounds/creature/hooved/{generic,large,medium,small}/` | — | Звуки копытных (по размеру/виду: elk, redstag, fawn) |
| `assets/survival/sounds/effect/` | 57 | Эффекты: взрывы, вода, станки, инструменты, портал, время |
| `assets/survival/sounds/environment/` | 15 | Окружение: ручей, капли, огонь, лава, водопад, вода, под водой |
| `assets/survival/sounds/held/` | 14 | Звуки предметов в руке (idle/указатель) |
| `assets/survival/sounds/instrument/` | 1 | Инструменты |
| `assets/survival/sounds/player/` | 27 | Звуки игрока: монеты, ремонт, крафт, кошение, давки и др. |
| `assets/survival/sounds/tool/` | 7 | Звуки инструментов |
| `assets/survival/sounds/walk/` | 35 | Шаги по поверхностям (трава, камень, лёд, снег, песок, вода, дерево…) |
| `assets/survival/sounds/walk/inside/leafy/` | 5 | Шаги внутри/по листве |
| `assets/survival/sounds/wearable/` | 13 | Звуки экипировки (обувь, наряды) |
| `assets/survival/sounds/weather/` | 7 | Погода: молнии (4 дальности), ветер (лиственный/без листьев), гром |
| `assets/survival/sounds/weather/tracks/` | 5 | Погодные «треки» (loop): дождь, град, треск |
| `assets/survival/sounds/voice/` | 1 | Голоса |
| `assets/survival/sounds/voice/{accordion,clarinet,harp,...}/` | 7 шт × 11 инструментов | Ноты/звуки каждого инструмента (по 7 нот на инструмент) |
| `assets/game/sounds/player/` | 26 | Базовые звуки игрока: build, collect, death, hurt, drink, eat, jump, throw, swim… |
| `assets/game/sounds/environment/` | 1 | `wind.ogg` — базовый ветер |
| `assets/game/sounds/voice/` | 8 | Базовые звуки голосовых/музыкальных |
| `assets/game/sounds/walk/` | 4 | Базовые шаги (default1..4) |
| `assets/survival/sounds/soundconfig.json` | — | Конфиг саунд-сетов (выборы из нескольких файлов + дефолтные звуки блоков) |

---

## 3. Конфиги (что описывают, какие поля менять)

### 3.1 `soundconfig.json` (в `game/` и `survival/`)

Определяет **sound-сеты** — наборы из нескольких файлов, из которых игра выбирает случайно, чтобы звук не повторялся:

```json
"soundsets": {
    "walk/grass": ["walk/grass1", "walk/grass2", "walk/grass3"],
    "player/hurt": ["player/hurt1", "player/hurt2", "player/hurt3", "player/hurt4"]
}
```
Каждое имя — путь **относительно `sounds/`**, без `.ogg`. Если заменять звук, то или меняешь файл под этим именем (самый простой путь), или меняешь ссылку здесь.

```json
"defaultBlockSounds": {
    "walk":  "walk/default",
    "break": "player/destruct",
    "hit":   "player/destruct",
    "place": "player/build"
}
```
Это **запасные звуки блоков**, которые подставляются блокам без своих `sounds`. Блоку в JSON можно задать свои (`"sounds": { "walk": "walk/wood" }`), тогда дефолт не применяется.

### 3.2 Как блок ссыла́ется на звук (пример из `blocktypes/.../trapdoor.json`)

```json
"attributes": {
    "openSound":  "sounds/block/door",   // полный путь к файлу (со звуком "sounds/")
    "closeSound": "sounds/block/door"
},
"sounds": {
    "place": "block/planks",             // относительный путь от sounds/, без .ogg
    "hit":   "block/planks",
    "break": "block/planks",
    "walk":  "walk/wood"
}
```
- Формат `"sounds"`: под-ключи `place` / `hit` / `break` / `walk` → путь **от папки `sounds/`**, расширение добавляется движком.
- Формат `"openSound"`/`closeSound` и др.: **полный путь** `sounds/...` (тоже без расширения).

---

## 4. Как заменить звук/трек (практически)

**Вариант А — «поверхностная» замена (рекомендую):**
1. Сохрани свой файл в формате **`.ogg`** (Vorbis). Совет: 44.1 кГц или 48 кГц, стерео или моно (движок поддерживает mono/stereo 8/16 бит; OGG-декодер сам разворачивает в PCM).
2. Имя файла — **точно как у оригинала**, **без** `.ogg` (расширение добавляет движок), **без** лишних пробелов в имени.
3. Скопируй в **тот же путь**.

**Вариант Б — смена ссылки:**
- Поменяй имя/путь в `soundconfig.json` / `musicconfig.json` / в JSON блока/сущности (см. §3.2).
- Если `file` в `musicconfig.json` указывает на несуществующий файл — игра может выдать ошибку в логе и пропустить трек.

**Вариант В — через мод (не трогая файлы игры):**
- Мод-паки перегружают ассеты. Создай мод, который кладёт свои `sounds/*.ogg` / `music/*.ogg` и/или переопределяет `musicconfig.json`. Тогда оригинал не затрагивается, замена «накладывается» (см. механику asset-загрузки).

**Важно:**
- Формат `.ogg`/`.wav` определяется по первым 4 байтам (`RIFF` → WAV, иначе → OGG). Если файл повреждён/не тот формат — в логе будет «Could not load sound ...» и звук не будет играть.
- Не меняй имена файлов, на которые ссылаются саунд-сеты (см. `soundconfig.json`), или обновляй и сеты.

---

## 5. Что проверять в игре после замены

### 5.1 Общая проверка
1. **Перезапусти игру** после замены файлов (ассеты загружаются при старте; замена на лету не подхватывается).
2. **Смотри лог:** `logs/latest-logs.txt` — ищи `Could not load sound`, `Failed to load`, `music`/`Ogg` ошибки. Это главный индикатор битых/неверных файлов.
3. **Настройки звука** (в игре → Options → Sound): ползунки **Music / Ambient / Entity / Weather / SFX** — по категориям (`EnumSoundType` → `MusicLevel` / `AmbientSoundLevel` / `EntitySoundLevel` / `WeatherSoundLevel` / `SoundLevel`). Убедись, что нужная категория не на нуле.
4. Сравни с оригиналом: включи игру до замены и запиши, как звучит каждая категория.

### 5.2 По категориям — конкретные действия в игре

**Блоки (`survival/sounds/block/`, `game/sounds/player/build|destruct`)**
- Ломание: ломать землю, дерево, камень, металл, стекло, керамику (каждый материал → свой файл, напр. `block/planks`, `block/glass`, `block/ceramicbreak`, `block/heavymetal-hit`).
- Удар: бить по блокам без поломки.
- Став́ка: ставить блоки (`player/build`, `block/planks` place).
- Двери/ящики/баррики: открывать-закрывать (`block/door`, `chestopen`, `barrel`, `metaldoor`).

**Шаги (`walk/` в `survival` и `game`)**
- Ходи по разным поверхностям: трава (`walk/grass*`), камень (`walk/stone*`), лёд (`walk/ice*`), снег (`walk/snow*`, `deepsnow*`), песок (`walk/sand*`), вода (`walk/water*`), дерево (`walk/wood*`), стекло (`walk/glass*`), грязь (`walk/sludge*`).

**Существа (`creature/`)**
- Подойди к каждому виду: медведь (`creature/bear`), курица (`creature/chicken`), коза (`creature/goat`), волк, лиса, барсук, свинья, шивер (шивэр/«shiver»), гидра, пчела (`beemob`, `beesting`), дрейфер (`drifter-idle/aggro/hurt/death`).
- Проверь состояния: idle (простой), aggro (нападение), hurt (ранен), death (смерть), еда (`animal-eat*`).

**Окружение (`environment/`)**
- Рядом с водой: ручей (`creek`), водопад (`waterfall`), волны (`waterwaves`), под водой (`underwater`), брызги (`largesplash`, `mediumsplash`, `smallsplash`).
- Капли в пещерах (`drip*`), огонь/костёр (`fire`, `fireplace`), лава (`lava`).
- Ветер (`game/sounds/environment/wind.ogg`).

**Погода (`weather/` + `weather/tracks/`)**
- Дождь: `rain-leafy` (с листвой) / `rain-leafless` (без), град (`hail`).
- Гром/молнии: 4 уровня близости (`lightning-verynear` / `near` / `distant` / `nodistance`), раскаты (`lowgrumble`, `lowtremble`, `verylowtremble`).
- Ветер: `wind-leafy` / `wind-leafless`.
- *Привести погоду:* `t`/время — или просто подожди/используй креатив-команды; или создай новый мир в нужное время.

**Эффекты (`effect/`)**
- Взрывы (`small/medium/largeexplosion`), вода (`water-pour`, `water-fill`, `watering`), станки (кузница, толкучка `crusher-impact`, гильотина), инструменты, портал/разрыв (`portal`, `rift`, `translocate-*`), `treefell` (упавшее дерево), `toolbreak` (сломанный инструмент).

**Музыка (`music/`)**
- Поверхность: меняй **часы суток** (команды или просто играй в разное время), **сезон** и **широту** — разные треки срабатывают по `minhour/maxhour/minSeason/minLatitude/maxTemperature`.
  - Утро: `night-to-day`, `to-dawn`, `spring`; день: `daylight`, `hallowcroft`, `summer-day`; вечер: `setting-sun`, `adventuring`; ночь: `midnight`, `through-the-grass-survive`, `groove`.
- Пещеры: иди в тёмную пещеру (свет < 12) → включится `CaveMusicTrack` (слои `deepunderground/*`), поверхностная музыка остановится.
- Event: войди в **Архив резонанса** (`schematicCode: "resonancearchive"`) → `theresonancearchives-*`.
- Creative-режим: заходи в creative → `heartbeat-create`, `sunny-village-create`, `peaceful-village`.

**Прочее**
- Инструменты/голоса (`voice/*`, `instrument/`): играй на инструментах.
- Предметы в руке (`held/`), одежда (`wearable/`).
- Игрок: сбор (`collect*`), еда (`eat*`), питьё (`drink*`), урон (`hurt*`), смерть (`death*`), прыжок, бросок, плавание.

---

## 6. Чек-лист «заменили → проверить»

- [ ] Файл сохранён в `.ogg` (Vorbis), имя совпадает с оригиналом **без** `.ogg`.
- [ ] Файл в правильном пути (`assets/{pack}/sounds/...` или `assets/{pack}/music/...`).
- [ ] `soundconfig.json` / `musicconfig.json` / JSON блоков не ссылаются на несуществующие имена.
- [ ] Игра **перезапущена**.
- [ ] В логе нет `Could not load sound` / `Failed to load` / ошибок OGG.
- [ ] В настройках звука соответствующая категория не на нуле.
- [ ] Звук реально проигрывается в той ситуации, в которой ожидается (см. §5.2).
- [ ] Громкость/длительность/тембр приемлемы (не режет, не слишком короткий/длинный).

---

## 7. Краткая карта путей (шпаргалка)

```
assets/
├─ game/
│  ├─ music/                 night-to-day, nostalgic, roots  (+ musicconfig.json)
│  └─ sounds/
│     ├─ environment/        wind.ogg
│     ├─ player/             build, collect, death, hurt, drink, eat, jump, throw, swim...
│     ├─ voice/              accordion, altoflute, clarinet, harmonica, oboe, sax, trumpet...
│     └─ walk/               default1..4
├─ survival/
│  ├─ music/                 41 треков поверхности/event (+ musicconfig.json)
│  │  ├─ deepunderground/    33 слоя пещерной музыки
│  │  └─ tuningcylinder/     4 трека резонанса
│  └─ sounds/                (+ soundconfig.json)
│     ├─ block/ (+ creak/)   звуки блоков
│     ├─ creature/ (+ подпапки по видам/копытным)
│     ├─ effect/             57 эффектов
│     ├─ environment/         ручей, огонь, лава, вода...
│     ├─ held/  instrument/  player/  tool/  voice/(+подпапки)  walk/(+inside)  wearable/
│     └─ weather/ (+ tracks/)
└─ creative/
   └─ music/                 heartbeat-create, sunny-village-create, ... (+ musicconfig.json)
```

---

## 8. Ссылки на механику (для понимания, как это работает внутри)

- [audio-core](../docs/mechanics/audio-core/README.md) — движок OpenAL, загрузка WAV/OGG, `LoadedSoundNative`, громкость по категориям (`EnumSoundType` → ползунки), fade, HRTF.
- [audio-ogg](../docs/mechanics/audio-ogg/README.md) — декодер OGG → PCM, dispatch `RIFF`/OGG (почему поддерживаются и `.ogg` и `.wav`).
- [audio-sounds](../docs/mechanics/audio-sounds/README.md) — `SystemSoundEngine`, позиционные звуки, реверб.
- [audio-ambient](../docs/mechanics/audio-ambient/README.md) — фоновые звуки (ветер, вода, пещеры).
- [audio-music](../docs/mechanics/audio-music/README.md) — музыкальный движок, `SurfaceMusicTrack`/`CaveMusicTrack`/`EventMusicTrack`, off-thread декод.

> Значение «688 файлов» и структура получены сканированием `assets/` этой конкретной сборки (v1.21.5). Если установишь другой патч/модификацию — перечисли папки заново.
