# Звуковое оформление «Былины и Мемы» — Полное руководство

> Документ содержит: инструкцию для FeralZombie, список всех SFX (~250+ звуков), музыкальных треков и песен с готовыми английскими промптами для ElevenLabs.
> 
> **Версия:** 1.0 | **Дата:** 2026-05-24 | **Бюджет:** 130 000 кредитов ElevenLabs

---

## Содержание

1. [Бюджет и распределение кредитов](#1-бюджет-и-распределение-кредитов)
2. [Инструкция для FeralZombie — как пользоваться ElevenLabs](#2-инструкция-для-feralzombie--как-пользоваться-elevenlabs)
3. [Категории звуков в игре](#3-категории-звуков-в-игре)
4. [Полный список SFX с промптами](#4-полный-список-sfx-с-промптами)
   - 4.1 Оружие и атаки
   - 4.2 Враги (куры, петухи, гуси, утки, барашки, пчёлы, муравьи)
   - 4.3 Боссы и супербоссы
   - 4.4 UI и меню
   - 4.5 Лут, подбор предметов, XP
   - 4.6 Окружение и амбиент
   - 4.7 Шаги и передвижение
   - 4.8 Способности и магия
   - 4.9 Кат-сцены и комиксы
   - 4.10 Смерть, Game Over, победа
   - 4.11 Специальные и редкие события
5. [Музыка и песни — список с промптами](#5-музыка-и-песни--список-с-промптами)
6. [Библиотека готовых промптов (копировать и вставлять)](#6-библиотека-готовых-промптов-копировать-и-вставлять)
7. [Технические советы и FAQ](#7-технические-советы-и-faq)

---

## 1. Бюджет и распределение кредитов

У вас **130 000 кредитов** ElevenLabs. Вот как их распределить разумно:

| Направление | Кредитов | Примечание |
|-------------|----------|------------|
| **Sound Effects (SFX)** | ~70 000 (~55%) | ~500 генераций × ~140 кредитов (auto) |
| **Музыка (Music)** | ~50 000 (~38%) | ~160 минут музыки |
| **Резерв** | ~10 000 (~7%) | На перегенерацию неудачных звуков |

### Что можно сгенерировать на 130 000 кредитов:

| Тип | Сколько получится |
|-----|-------------------|
| Sound Effects генерации (auto-duration) | ~500 генераций = **~2000 вариантов звуков** (по 4 варианта за генерацию) |
| Sound Effects с фикс. длительностью (2сек) | ~875 звуков (по 40 кредитов/сек × 2сек) |
| Музыкальные треки (по 2 минуты) | **~80+ треков** |
| Музыкальные треки (по 3 минуты) | **~55 треков** |

**Вывод:** Бюджета с запасом хватит на ВСЕ звуки и музыку для MVP + полировку.

---

## 2. Инструкция для FeralZombie — как пользоваться ElevenLabs

### Шаг 1: Регистрация и вход

1. Открыть сайт: **https://elevenlabs.io**
2. Нажать **Sign up** (регистрация через Google/email)
3. Подтвердить email
4. Зайти в личный кабинет

### Шаг 2: Генерация Sound Effects (звуков)

1. В боковом меню слева нажать **Sound Effects** (раздел Playground)
   - Прямая ссылка: https://elevenlabs.io/app/sound-effects

2. **В текстовое поле вставить промпт** (на английском!)
   - Максимум 450 символов
   - Чем конкретнее — тем лучше результат

3. **Настроить параметры:**

| Параметр | Что значит | Рекомендация для нашей игры |
|----------|-----------|----------------------------|
| **Duration** | Длительность звука | Короткие SFX: 1-2 сек. Ambient: 10-20 сек. Оставить `Auto` для простых звуков |
| **Looping** | Зацикливание | Включать ТОЛЬКО для ambient (дождь, ветер, костёр). Для остальных — выключено |
| **Prompt Influence** | Насколько строго AI следует промпту | **0.7-0.9** для точных звуков (удары, шаги). **0.3-0.5** для креативных (магия, странные звуки) |

4. Нажать стрелку **Generate** (справа от поля)

5. Получишь **4 варианта** звука — прослушай все

6. **Сохранение:**
   - Нажать **звёздочку** чтобы добавить в Favorites
   - Нажать **скачать** и выбрать формат:
     - **WAV 48kHz** — для финальных ассетов (лучшее качество)
     - **MP3 44.1kHz** — если нужно экономить место

7. Если результат не нравится — **подкорректируй промпт** и нажми Generate снова

### Шаг 3: Генерация Music (музыки и песен)

1. В боковом меню нажать **Music**
   - Прямая ссылка: https://elevenlabs.io/app/music

2. **Вставить промпт** в текстовое поле (описание трека)

3. **Настройки:**
   - **Duration:** до 5 минут максимум (300 секунд)
   - **Instrumental only** — если нужен instrumental без вокала
   - **Lyrics** — если нужна песня со словами (напиши текст или оставь пустым — AI сам придумает)
   - **Stems** — можно генерировать отдельные дорожки ( drums, bass, melody)

4. Нажать **Generate**

5. Музыка генерируется дольше звуков (1-3 минуты ожидания)

6. **Скачивание:** MP3 или WAV

### Шаг 4: Проверка баланса кредитов

- Нажать на **иконку профиля** (справа вверху)
- Выбрать **Subscription** или **Usage**
- Там видно сколько кредитов осталось

### Золотые правила для лучших результатов:

1. **ВСЕГДА пиши промпты на английском** — результат в 10 раз лучше, чем на русском
2. **Используй формулу:** Subject + Action + Scene + Quality
   - Пример: `axe whooshing through air, sharp swing, medieval combat, impactful`
3. **Добавляй стилевые теги:** `pixel art game`, `8-bit retro`, `cartoon style`, `cinematic`
4. **Избегай абстрактных слов** — не пиши "good sound", "nice effect". Вместо этого: `sharp metallic impact with echo`
5. **Генерируй по 3-5 версий** одного звука — каждый раз AI выдаёт разный результат
6. **Короткие звуки = 1-2 секунды.** Ambient = 10-20 секунд. Музыка = 2-3 минуты.
7. **Сохраняй хорошие звуки в Favorites** — чтобы не потерять
8. **Именуй файлы сразу:** `sfx_axe_swing_v1.wav`, `music_boss_petukh_loop.wav`
9. **Looping включаем ТОЛЬКО для:** дождь, ветер, костёр, фоновая музыка
10. **Если звук "фальшивый"** — увеличь Prompt Influence до 0.8-1.0

### Структура промпта для идеального результата:

```
[Subject: что издаёт звук] + [Action: что делает] + [Scene: контекст] + [Quality: качество/стиль]
```

**Примеры:**
- ✅ `sharp metallic axe swing through air, whoosh, pixel art game combat, impactful`
- ✅ `chicken clucking loudly, farmyard ambience, cartoon style, funny`
- ❌ `axe sound` — слишком коротко и абстрактно
- ❌ `хороший звук удара` — на русском, нет деталей

---

## 3. Категории звуков в игре

Всего в игре **11 категорий** звуков:

| # | Категория | Кол-во | Описание |
|---|-----------|--------|----------|
| 1 | Оружие и атаки | ~30 | Все виды оружия (топор, коса, метла, тарелки, пирожки, пистолет, кнут и т.д.) |
| 2 | Враги | ~60 | Звуки кур, петухов, гусей, уток, барашек, пчёл, муравьёв |
| 3 | Боссы и супербоссы | ~25 | Петух, Баран, Бабка, Внучка, Жучка, Кошка, Мышка |
| 4 | UI и меню | ~20 | Клики, наведение, открытие меню, пауза, настройки |
| 5 | Лут, подбор, XP | ~15 | Звуки подбора яиц, монет, XP, магнита, левел-ап |
| 6 | Окружение (Ambient) | ~20 | Деревня, дождь, ветер, колодец, петухи на рассвете |
| 7 | Шаги и передвижение | ~15 | По траве, грядкам, доскам, грязи |
| 8 | Способности и магия | ~20 | Взрывы, лед, огонь, электричество, баффы |
| 9 | Кат-сцены и комиксы | ~10 | Переходы, появление панелей, диалоги |
| 10 | Смерть, Game Over, победа | ~15 | Смерть врагов, Game Over, победа над боссом |
| 11 | Специальные события | ~15 | Редкие дропы, секреты, пасхалки, ачивки |
| | **ИТОГО:** | **~245 звуков** | |

---

## 4. Полный список SFX с промптами

> **Формат:** `Название (RU) | Название файла | Промпт (EN) | Duration | Prompt Influence`

---

### 4.1 Оружие и атаки (30 звуков)

#### Дед — Топор

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 1 | Топор: бросок | `sfx_axe_throw_01` | `sharp metallic throwing axe whooshing through air, combat swing, pixel art game, impactful` | 1.5s | 0.8 |
| 2 | Топор: попадание | `sfx_axe_hit_01` | `heavy axe hitting flesh with squish impact, cartoon gore, pixel game combat` | 1.0s | 0.9 |
| 3 | Топор: попадание в дерево | `sfx_axe_hit_wood` | `axe embedded in wooden log, thud with splintering wood crack` | 1.0s | 0.8 |
| 4 | Топар: эволюция (огненный) | `sfx_axe_fire_01` | `flaming axe swing with fire whoosh, blazing trail, RPG upgrade, sizzling` | 2.0s | 0.7 |
| 5 | Топор: удар по земле | `sfx_axe_ground` | `battle axe slamming ground with heavy impact, earth shake, dust burst` | 1.5s | 0.8 |

#### Дед — Коса

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 6 | Коса: вращение | `sfx_scythe_spin_01` | `scythe blade spinning rapidly, sharp metallic whirlwind, circular swing, dark fantasy` | 2.0s | 0.8 |
| 7 | Коса: удар | `sfx_scythe_hit_01` | `scythe slicing through multiple enemies, sharp slash, harvest reaper` | 1.0s | 0.9 |
| 8 | Коса: эволюция | `sfx_scythe_death_01` | `death scythe ethereal swing, ghostly wail, dark magic, spectral trail` | 2.5s | 0.6 |

#### Бабка — Метла

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 9 | Метла: взмах | `sfx_broom_sweep_01` | `witch broom sweeping through air, magical whoosh, cartoon fantasy, bristle rustle` | 1.5s | 0.8 |
| 10 | Метла: удар волной | `sfx_broom_cone_01` | `broom creating cone of sweeping wind, magical gust, dust particles, sweeping force` | 2.0s | 0.7 |
| 11 | Метла: эволюция (ядовитая) | `sfx_broom_poison_01` | `poisonous broom leaving green toxic trail, bubbling acid hiss, witch magic, venomous` | 2.5s | 0.6 |

#### Бабка — Тарелка

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 12 | Тарелка: бросок | `sfx_plate_throw_01` | `ceramic plate spinning through air, frisbee whir, kitchen combat, comical` | 1.5s | 0.8 |
| 13 | Тарелка: попадание/разбивание | `sfx_plate_break_01` | `plate smashing against wall with loud ceramic shatter, crash debris, cartoon destruction` | 1.5s | 0.9 |
| 14 | Тарелка: эволюция (фарфор) | `sfx_plate_porcelain_01` | `porcelain plate bouncing between three targets, magical ping pong ricochet, crystal chime` | 2.0s | 0.7 |

#### Бабка — Пирожок

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 15 | Пирожок: бросок | `sfx_pirozhok_throw_01` | `pastry projectile flying through air, soft whoosh, silly cartoon food weapon` | 1.5s | 0.7 |
| 16 | Пирожок: взрыв/попадание | `sfx_pirozhok_explode_01` | `hot pastry explosion with steam burst, food splat, comical sizzle, cartoon combat` | 1.5s | 0.8 |
| 17 | Пирожок: эволюция (горячий) | `sfx_pirozhok_fire_01` | `flaming pie explosion with fire burst and pastry debris, volcanic baked good, scorching` | 2.0s | 0.7 |

#### Внучка — Водяной пистолет

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 18 | Водяной пистолет: выстрел | `sfx_watergun_shoot_01` | `water pistol squirt, liquid splash projectile, toy gun, cartoon water jet` | 1.0s | 0.8 |
| 19 | Водяной пистолет: попадание | `sfx_watergun_hit_01` | `water splash hitting target with wet impact, dripping soak, cartoon splash` | 1.0s | 0.8 |
| 20 | Пистолет: эволюция | `sfx_watergun_super_01` | `super soaker high-pressure water beam, powerful hydro blast, RPG upgrade, torrent` | 2.0s | 0.7 |

#### Внучка — Кнут

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 21 | Кнут: взмах | `sfx_whip_crack_01` | `leather whip cracking through air, sharp snap, Indiana Jones style, loud crack` | 1.0s | 0.9 |
| 22 | Кнут: удар | `sfx_whip_hit_01` | `whip lashing enemy with sting impact, leather snap hit, painful smack` | 1.0s | 0.8 |
| 23 | Кнут: эволюция (бычий) | `sfx_whip_bull_01` | `bullwhip thunder crack with echo, deafening snap, legendary weapon, stun effect` | 1.5s | 0.8 |

#### Внучка — Ракетка

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 24 | Ракетка: вращение вокруг | `sfx_racket_orbit_01` | `badminton racket orbiting around player, rapid swishing rotation, sporty weapon` | 2.0s | 0.7 |
| 25 | Ракетка: удар | `sfx_racket_hit_01` | `badminton racket smashing shuttlecock, sharp sports impact, satisfying pop` | 1.0s | 0.8 |

#### Жучка — Блохи

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 26 | Блохи: прыжок/появление | `sfx_fleas_spawn_01` | `fleas hopping and biting, tiny insect swarm, itchy scratchy sound, gross comedy` | 1.5s | 0.6 |
| 27 | Блохи: укус | `sfx_fleas_bite_01` | `flea bite tiny pinch with itch squeak, miniature damage, swarm attack` | 0.5s | 0.8 |

#### Жучка — Вонь

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 28 | Вонь: облако | `sfx_stink_cloud_01` | `toxic stink cloud expanding, green gas hiss, foul odor vapour, comical pollution, gross` | 2.5s | 0.6 |
| 29 | Вонь: эволюция | `sfx_stink_ultimate_01` | `devastating fart explosion with toxic green wave, biohazard gas, ultimate ability, comical` | 3.0s | 0.5 |

#### Жучка — Цепь

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 30 | Цепь: взмах | `sfx_chain_whip_01` | `metal chain whipping through air, heavy iron links clanking, brutal swing` | 1.5s | 0.8 |
| 31 | Цепь: удар | `sfx_chain_hit_01` | `chain smashing enemy with heavy metal impact, bone crush, brutal damage` | 1.0s | 0.9 |

---

### 4.2 Враги — звуки (60 звуков)

#### Куры (3 цвета)

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 32 | Курица: кудахтанье | `sfx_chicken_cluck_01` | `hen clucking happily, farmyard chicken vocalization, cartoon poultry, funny` | 1.5s | 0.6 |
| 33 | Курица: крик (паника) | `sfx_chicken_panic_01` | `chicken panicking with loud squawk, distressed poultry flapping, alarmed bird` | 1.5s | 0.7 |
| 34 | Курица: удар крылом | `sfx_chicken_flap_01` | `chicken wings flapping rapidly, feather rustle, bird taking off, cartoon` | 1.0s | 0.7 |
| 35 | Курица: смерть | `sfx_chicken_death_01` | `chicken dying with comical squawk and feather poof, poultry defeat, funny death` | 1.5s | 0.6 |
| 36 | Курица: клюв/атака | `sfx_chicken_peck_01` | `chicken pecking attack, sharp beak jab, bird strike, cartoon combat` | 0.8s | 0.8 |
| 37 | Курица: шаги | `sfx_chicken_steps_01` | `chicken walking with tiny claw steps, bird feet scratching ground, farm` | 1.0s | 0.7 |
| 38 | Курица: шипение (злая) | `sfx_chicken_hiss_01` | `angry chicken hissing aggressively, mad poultry, territorial bird, funny scary` | 1.5s | 0.6 |

#### Петух (мини-босс + обычный)

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 39 | Петух: кукареканье | `sfx_rooster_crow_01` | `rooster crowing loudly at dawn, classic cock-a-doodle-doo, farm morning` | 2.5s | 0.7 |
| 40 | Петух: боевой крик | `sfx_rooster_battlecry_01` | `rooster battle cry with aggressive crow, fierce poultry warrior, intimidating bird` | 2.0s | 0.7 |
| 41 | Петух: рывок/атака | `sfx_rooster_charge_01` | `rooster charging with feather ruffle and aggressive clucking, bird dash` | 1.5s | 0.7 |
| 42 | Петух: удар шпорами | `sfx_rooster_spur_01` | `rooster spur slash, sharp talon strike, chicken claw attack, painful jab` | 1.0s | 0.8 |
| 43 | Петух: круговая волна (крик) | `sfx_rooster_shockwave_01` | `rooster screaming with sonic shockwave blast, loud crow explosion, AOE attack` | 2.5s | 0.6 |
| 44 | Петух: призыв куриц | `sfx_rooster_summon_01` | `rooster calling hens with commanding crow, poultry leader rally, summoning` | 2.0s | 0.6 |
| 45 | Петух: ранен | `sfx_rooster_hurt_01` | `rooster hurt with pained crow, damaged poultry warrior, weak cluck` | 1.5s | 0.6 |
| 46 | Петух: смерть | `sfx_rooster_death_01` | `rooster dying with dramatic final crow, poultry boss defeated, comical tragedy` | 2.5s | 0.5 |

#### Гуси (3 цвета)

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 47 | Гусь: гоготание | `sfx_goose_honk_01` | `goose honking aggressively, angry goose hiss-honk, territorial waterfowl, funny` | 2.0s | 0.6 |
| 48 | Гусь: шипение | `sfx_goose_hiss_01` | `goose hissing with neck extended, threatening waterfowl, scary goose` | 1.5s | 0.6 |
| 49 | Гусь: удар крылом | `sfx_goose_wing_01` | `goose wing slap, powerful feather hit, waterfowl attack, heavy flap strike` | 1.0s | 0.8 |
| 50 | Гусь: шаги | `sfx_goose_steps_01` | `goose webbed feet walking on grass, duck waddle steps, heavy bird walking` | 1.0s | 0.7 |
| 51 | Гусь: смерть | `sfx_goose_death_01` | `goose defeated with sad honk, waterfowl dying, comical goose tragedy` | 2.0s | 0.5 |

#### Утка

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 52 | Утка: кряканье | `sfx_duck_quack_01` | `duck quacking rapidly, classic duck vocalization, cartoon waterfowl, funny` | 1.5s | 0.6 |
| 53 | Утка: зигзаг-рывок | `sfx_duck_dash_01` | `duck dashing in zigzag with rapid wing flutter, erratic waterfowl movement` | 1.5s | 0.7 |
| 54 | Утка: брызги | `sfx_duck_splash_01` | `duck splashing water, wet spray burst, puddle splash, muddy wave` | 1.5s | 0.7 |
| 55 | Утка: смерть | `sfx_duck_death_01` | `duck dying with fading quack, waterfowl defeated, comical duck tragedy` | 1.5s | 0.5 |

#### Барашки (3 цвета)

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 56 | Барашек: блеяние | `sfx_sheep_baa_01` | `sheep lamb bleating softly, cute farm animal, woolly baa, cartoon` | 1.5s | 0.6 |
| 57 | Барашек: стадное блеяние | `sfx_sheep_herd_01` | `flock of sheep bleating together, multiple farm animals, herd chaos` | 2.5s | 0.5 |
| 58 | Барашек: толчок/таран | `sfx_sheep_ram_01` | `sheep headbutt charge, woolly body slam, ram impact, cartoon bump` | 1.0s | 0.8 |
| 59 | Барашек: шаги | `sfx_sheep_steps_01` | `sheep hooves walking on grass, soft padded animal steps, farmyard` | 1.0s | 0.7 |
| 60 | Барашек: смерть | `sfx_sheep_death_01` | `sheep defeated with sad final baa, cute animal dying, woolly poof` | 1.5s | 0.5 |

#### Баран (мини-босс)

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 61 | Баран: рёв | `sfx_ram_roar_01` | `ram bellowing aggressively, angry male sheep roar, big horns charging` | 2.0s | 0.7 |
| 62 | Баран: таран (рывок) | `sfx_ram_charge_01` | `ram charging with heavy hoof beats, horned tackle, powerful beast dash` | 2.0s | 0.8 |
| 63 | Баран: удар рогами | `sfx_ram_horn_01` | `ram horns crashing into target with heavy impact, bone shatter, powerful hit` | 1.0s | 0.9 |
| 64 | Баран: дрожание земли | `sfx_ram_earthquake_01` | `heavy ram stomping causing earth tremor, ground shake rumble, powerful shockwave` | 2.5s | 0.7 |
| 65 | Баран: неуязвимость | `sfx_ram_armor_01` | `ram glowing with protective aura, iron skin shimmer, invincibility buff, metallic` | 2.0s | 0.6 |
| 66 | Баран: ранен | `sfx_ram_hurt_01` | `ram hurt with angry pained bellow, damaged boss, weakened roar` | 1.5s | 0.6 |
| 67 | Баран: смерть | `sfx_ram_death_01` | `ram boss dying with massive collapse, heavy beast falling, ground thud, epic` | 2.5s | 0.7 |

#### Пчёлы

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 68 | Пчела: жужжание | `sfx_bee_buzz_01` | `bee buzzing angrily, insect wing vibration, aggressive honeybee, annoying` | 1.5s | 0.6 |
| 69 | Пчела: рой | `sfx_bee_swarm_01` | `swarm of bees buzzing together, multiple insect wings, threatening hive` | 2.5s | 0.5 |
| 70 | Пчела: укус/жало | `sfx_bee_sting_01` | `bee stinging with sharp needle prick, poison injection, tiny painful jab` | 0.5s | 0.8 |
| 71 | Пчела: вылет из улья | `sfx_bee_spawn_01` | `bees pouring out of wooden hive, honeycomb break, swarm emergence` | 2.0s | 0.6 |
| 72 | Пчела: смерть | `sfx_bee_death_01` | `single bee dying with tiny buzz fade, insect defeated, small poof` | 0.8s | 0.6 |

#### Муравьи

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 73 | Муравей: шаги (рой) | `sfx_ant_march_01` | `ants marching in formation, many tiny legs marching, insect army steps` | 1.5s | 0.7 |
| 74 | Муравей: укус | `sfx_ant_bite_01` | `ant bite tiny pinch, miniature insect attack, small nibble` | 0.5s | 0.7 |
| 75 | Муравей: появление из муравейника | `sfx_ant_spawn_01` | `ants emerging from anthill mound, dirt crumbling, insect swarm pouring out` | 2.0s | 0.6 |
| 76 | Муравей: смерть (пачка) | `sfx_ant_squish_01` | `ants being squished with crunch, multiple insect crush, small crackle` | 1.0s | 0.8 |

#### Общие звуки врагов

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 77 | Враг: получение урона (общее) | `sfx_enemy_hurt_01` | `enemy taking damage, generic creature hit, cartoon pain squeak` | 0.8s | 0.7 |
| 78 | Враг: критический удар | `sfx_enemy_crit_01` | `critical hit with exaggerated impact, heavy damage, screen shake sound, powerful` | 1.0s | 0.8 |
| 79 | Враг: появление (спавн) | `sfx_enemy_spawn_01` | `enemy spawning with puff of smoke, materialization poof, cartoon appear` | 1.0s | 0.7 |
| 80 | Враг: моргание/мерцание при уроне | `sfx_enemy_flash_01` | `enemy flashing white when hit, damage flicker sound, hit confirmation beep` | 0.3s | 0.8 |
| 81 | Враг: заморозка (стан) | `sfx_enemy_freeze_01` | `enemy being frozen in ice, crystal encasement, shatter prelude, ice magic` | 1.5s | 0.7 |
| 82 | Враг: горение (DOT) | `sfx_enemy_burn_01` | `enemy burning with fire crackle, sizzle damage, flame tick, roasting` | 1.5s | 0.6 |
| 83 | Враг: отравление (DOT) | `sfx_enemy_poison_01` | `enemy poisoned with bubbling acid, toxic damage tick, green corrosion hiss` | 1.0s | 0.6 |
| 84 | Враг: уклонение | `sfx_enemy_dodge_01` | `enemy dodging attack with swift whoosh, miss sound, evasion swoosh` | 0.8s | 0.7 |
| 85 | Враг: спавн-волна (много) | `sfx_wave_spawn_01` | `large wave of enemies spawning, multiple poofs, swarm arrival, ominous` | 2.0s | 0.6 |
| 86 | Враг: дроп предмета | `sfx_enemy_drop_01` | `enemy dropping loot with coin jingle, item falling, reward sparkle` | 1.0s | 0.7 |
| 87 | Враг: дроп яйца (курица) | `sfx_egg_drop_01` | `chicken laying egg with soft thud, egg hitting ground, farm drop` | 0.8s | 0.7 |
| 88 | Враг: дроп пера (гусь) | `sfx_feather_drop_01` | `feather floating down gently, soft landing, light plume drop` | 0.8s | 0.5 |
| 89 | Враг: дроп шерсти (баран) | `sfx_wool_drop_01` | `wool tuft falling with soft fluffy thud, sheep fleece drop` | 0.8s | 0.6 |
| 90 | Враг: дроп жала (пчела) | `sfx_stinger_drop_01` | `bee stinger dropping with small metallic ping, tiny needle fall` | 0.5s | 0.7 |
| 91 | Враг: дроп листочка (муравей) | `sfx_leaf_drop_01` | `small leaf floating down gently, nature item drop, light rustle` | 0.8s | 0.5 |

---

### 4.3 Боссы и супербоссы (25 звуков)

#### Босс: Петух (Этап 1)

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 92 | Петух: появление | `sfx_boss_petukh_spawn_01` | `giant rooster boss emerging with dramatic fanfare, epic poultry arrival, boss intro` | 3.0s | 0.7 |
| 93 | Петух: боевой крик (вступление) | `sfx_boss_petukh_roar_01` | `massive rooster war cry, epic boss battle start, intimidating bird king, cinematic` | 3.0s | 0.7 |
| 94 | Петух: рывок-атака | `sfx_boss_petukh_dash_01` | `giant rooster dashing at player with wind whoosh, boss charge, feather trail` | 1.5s | 0.8 |
| 95 | Петух: круговая волна (ультимейт) | `sfx_boss_petukh_aoe_01` | `rooster boss screaming sonic shockwave, circular blast, epic AOE, screen shake` | 2.5s | 0.7 |
| 96 | Петух: призыв куриц (волна) | `sfx_boss_petukh_summon_01` | `boss rooster summoning chicken minions, commanding crow echo, reinforcements` | 2.0s | 0.6 |
| 97 | Петух: ранен (фаза 2) | `sfx_boss_petukh_phase2_01` | `rooster boss enraged, second phase transformation, angry power up, boss rage` | 2.5s | 0.6 |
| 98 | Петух: смерть (победа) | `sfx_boss_petukh_death_01` | `giant rooster boss dying with epic final crow, boss defeat, victory explosion` | 3.0s | 0.7 |

#### Босс: Утка (Этап 2)

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 99 | Утка: появление | `sfx_boss_utka_spawn_01` | `giant duck boss surfacing from water, epic waterfowl arrival, splash boss intro` | 3.0s | 0.7 |
| 100 | Утка: зигзаг-рывок | `sfx_boss_utka_dash_01` | `duck boss zigzag charge with water spray, erratic boss movement, slippery dash` | 1.5s | 0.8 |
| 101 | Утка: брызги (замедление) | `sfx_boss_utka_slow_01` | `duck boss splashing mud wave, player slowing goo, sticky water splash, swamp` | 2.0s | 0.7 |
| 102 | Утка: смерть | `sfx_boss_utka_death_01` | `giant duck boss defeated with water splash explosion, sinking quack, epic death` | 3.0s | 0.6 |

#### Босс: Баран (Этап 3)

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 103 | Баран: появление | `sfx_boss_ram_spawn_01` | `giant ram boss charging through gate, horned beast arrival, earth shaking intro` | 3.0s | 0.8 |
| 104 | Баран: таран-атака | `sfx_boss_ram_charge_01` | `ram boss full speed charge with ground cracking, devastating tackle, boss impact` | 2.0s | 0.9 |
| 105 | Баран: дрожание земли (ульт) | `sfx_boss_ram_quake_01` | `ram boss stomping causing massive earthquake, ground fissure, AOE tremor, epic` | 3.0s | 0.7 |
| 106 | Баран: броня (неуязвим) | `sfx_boss_ram_shield_01` | `ram boss iron skin activation, metallic glow, invincibility buff, clanging armor` | 2.0s | 0.7 |
| 107 | Баран: смерть | `sfx_boss_ram_death_01` | `giant ram boss collapsing with massive earth thud, horned beast defeated, epic` | 3.0s | 0.7 |

#### Супербосс: Бабка

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 108 | Бабка: появление (смех) | `sfx_super_granny_spawn_01` | `evil witch granny cackling laugh, scary old woman cackle, boss intro, horror comedy` | 3.0s | 0.6 |
| 109 | Бабка: полёт на метле | `sfx_super_granny_broom_01` | `witch granny flying on broomstick whoosh, magical sweep, evil flight, Halloween` | 2.0s | 0.7 |
| 110 | Бабка: взмах метлы (конус) | `sfx_super_granny_sweep_01` | `granny broom sweeping magical wind cone, gust blast, witch attack, sparkling dust` | 2.0s | 0.7 |
| 111 | Бабка: бросок тарелки | `sfx_super_granny_plate_01` | `granny throwing plate like frisbee, spinning dish projectile, kitchen witch` | 1.5s | 0.8 |
| 112 | Бабка: ранена (злость) | `sfx_super_granny_angry_01` | `granny boss getting angry, enraged old woman scream, furious babushka, scary` | 2.0s | 0.6 |
| 113 | Бабка: смерть (поражение) | `sfx_super_granny_defeat_01` | `witch granny defeated falling off broom, comical old woman defeat, poof vanish` | 3.0s | 0.6 |

#### Супербосс: Внучка

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 114 | Внучка: появление | `sfx_super_girl_spawn_01` | `cheeky girl appearing with giggle, playful child boss intro, mischievous laugh` | 2.0s | 0.5 |
| 115 | Внучка: выстрел водой | `sfx_super_girl_water_01` | `girl firing water pistol rapid shots, squirt squirt squirt, playful water attack` | 1.5s | 0.7 |
| 116 | Внучка: кнут-удар | `sfx_super_girl_whip_01` | `child cracking whip, leather snap, surprisingly powerful, playful combat` | 1.0s | 0.8 |
| 117 | Внучка: уклонение (смех) | `sfx_super_girl_dodge_01` | `girl giggling while dodging, child evasion with playful laugh, nimble kid` | 1.0s | 0.5 |
| 118 | Внучка: смерть (обида) | `sfx_super_girl_defeat_01` | `girl boss defeated with sad pout, childish tantrum, comical kid defeat, unfair` | 2.0s | 0.5 |

#### Супербосс: Жучка (собака)

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 119 | Жучка: появление (лай) | `sfx_super_dog_spawn_01` | `dog boss appearing with loud aggressive bark, territorial hound, angry puppy` | 2.0s | 0.7 |
| 120 | Жучка: рычание | `sfx_super_dog_growl_01` | `dog growling menacingly, low rumbling canine threat, aggressive guard dog` | 2.0s | 0.7 |
| 121 | Жучка: прыжок-атака | `sfx_super_dog_jump_01` | `dog leaping at player with bark attack, canine lunge, bite snap` | 1.5s | 0.8 |
| 122 | Жучка: вой (стан) | `sfx_super_dog_howl_01` | `dog howling with sonic stun effect, painful ears, AOE howl, wolf cry` | 2.5s | 0.6 |
| 123 | Жучка: блохи (спавн) | `sfx_super_dog_fleas_01` | `dog shaking off flea swarm, insect cloud spreading, gross bug attack, itching` | 2.0s | 0.5 |
| 124 | Жучка: смерть (скуление) | `sfx_super_dog_defeat_01` | `dog boss defeated with whining whimper, sad puppy defeat, tail between legs` | 2.0s | 0.5 |

#### Супербосс: Кошка

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 125 | Кошка: появление (мяуканье) | `sfx_super_cat_spawn_01` | `cat boss appearing with eerie meow, mysterious feline, creepy kitty intro` | 2.0s | 0.5 |
| 126 | Кошка: шипение | `sfx_super_cat_hiss_01` | `cat hissing aggressively with arched back, angry feline, territorial cat fight` | 1.5s | 0.7 |
| 127 | Кошка: царапина (когти) | `sfx_super_cat_claw_01` | `cat claw slash, sharp feline scratch, fast swiping attack, nail rip` | 1.0s | 0.8 |
| 128 | Кошка: шерсть (пуш-атака) | `sfx_super_cat_hairball_01` | `cat coughing up giant hairball projectile, disgusting fur ball, gross feline attack` | 2.0s | 0.5 |
| 129 | Кошка: мурлыкание (хил) | `sfx_super_cat_purr_01` | `cat purring with healing aura, gentle vibration, restorative feline magic, soothing` | 2.0s | 0.4 |
| 130 | Кошка: смерть | `sfx_super_cat_defeat_01` | `cat boss defeated with sad meow, falling gracefully, nine lives joke, poof` | 2.0s | 0.5 |

#### Супербосс: Мышка

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 131 | Мышка: появление (писк) | `sfx_super_mouse_spawn_01` | `tiny mouse boss appearing with squeak, miniature villain, cute rodent intro` | 1.5s | 0.5 |
| 132 | Мышка: мышеловка (ловушка) | `sfx_super_mouse_trap_01` | `mousetrap snapping shut with metallic clack, trap trigger, cheese bait spring` | 1.0s | 0.8 |
| 133 | Мышка: орех (снаряд) | `sfx_super_mouse_nut_01` | `nut projectile flying and bouncing, small hard object ricochet, acorn bullet` | 1.0s | 0.7 |
| 134 | Мышка: смерть | `sfx_super_mouse_defeat_01` | `tiny mouse boss defeated with cute squeak, small poof, rodent tragedy` | 1.5s | 0.5 |

---

### 4.4 UI и меню (20 звуков)

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 135 | UI: клик по кнопке | `sfx_ui_click_01` | `soft UI button click, subtle interface tap, pixel game menu select, gentle pop` | 0.5s | 0.7 |
| 136 | UI: наведение на кнопку | `sfx_ui_hover_01` | `UI hover tick, gentle interface rollover sound, soft blip, menu highlight` | 0.3s | 0.6 |
| 137 | UI: открытие меню | `sfx_ui_open_01` | `menu panel sliding open with paper rustle, interface unfold, whoosh reveal` | 1.0s | 0.6 |
| 138 | UI: закрытие меню | `sfx_ui_close_01` | `menu panel closing with soft snap, interface fold away, reverse whoosh` | 0.8s | 0.6 |
| 139 | UI: переключение вкладки | `sfx_ui_tab_01` | `tab switching with soft click, menu category change, clean interface select` | 0.5s | 0.7 |
| 140 | UI: включение паузы | `sfx_ui_pause_01` | `pause menu activating with time freeze effect, glass shimmer, game paused chime` | 1.5s | 0.6 |
| 141 | UI: выключение паузы | `sfx_ui_unpause_01` | `unpausing with time resume whoosh, game continue effect, reverse shimmer` | 1.0s | 0.6 |
| 142 | UI: ошибка/нельзя | `sfx_ui_error_01` | `error buzzer, cannot perform action, denied beep, wrong move buzz, error` | 0.8s | 0.7 |
| 143 | UI: слайдер (перетаскивание) | `sfx_ui_slider_01` | `slider knob moving with tick-tick-tick, volume adjustment, setting change ticks` | 0.5s | 0.6 |
| 144 | UI: галочка/подтверждение | `sfx_ui_confirm_01` | `confirmation checkmark with positive chime, success click, agree ding, pleasant` | 0.5s | 0.7 |
| 145 | UI: возврат/назад | `sfx_ui_back_01` | `back button with reverse swoosh, return to previous menu, cancel sound` | 0.5s | 0.6 |
| 146 | UI: покупка/прокачка | `sfx_ui_upgrade_01` | `meta-upgrade purchase with coin jingle and power chime, buying skill, positive` | 1.5s | 0.7 |
| 147 | UI: достижение разблокировано | `sfx_ui_unlock_01` | `achievement unlocked with triumphant fanfare, reward sparkle, celebration chime` | 2.0s | 0.6 |
| 148 | UI: новый герой открыт | `sfx_ui_hero_unlock_01` | `new hero unlocked with epic reveal fanfare, character summon, dramatic chord` | 2.5s | 0.7 |
| 149 | UI: смена персонажа | `sfx_ui_hero_switch_01` | `character switch with magical transition, hero swap whoosh, sparkling change` | 1.0s | 0.6 |
| 150 | UI: нажатие кнопки старт | `sfx_ui_start_01` | `game start button with energetic whoosh, run begin, adventure launch` | 1.5s | 0.7 |
| 151 | UI: таймер (отсчёт) | `sfx_ui_timer_01` | `timer countdown tick tock, time running out, urgent clock beat, pulse` | 0.5s | 0.7 |
| 152 | UI: таймер (последние 10 сек) | `sfx_ui_timer_final_01` | `urgent final countdown with fast ticking, time almost up, panic beeps, intense` | 2.0s | 0.8 |
| 153 | UI: карта ачивки (всплытие) | `sfx_ui_achievement_pop_01` | `achievement toast popup with short celebratory chime, notification slide in` | 1.0s | 0.6 |
| 154 | UI: настройки применены | `sfx_ui_apply_01` | `settings saved with soft confirmation chime, configuration applied, success` | 0.8s | 0.6 |

---

### 4.5 Лут, подбор предметов, XP (15 звуков)

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 155 | Лут: подбор яйца | `sfx_pickup_egg_01` | `egg pickup with soft pop and squish, oval item collect, gentle grab` | 0.5s | 0.7 |
| 156 | Лут: подбор монеты | `sfx_pickup_coin_01` | `coin pickup with bright metallic chime, gold collect sparkle, satisfying ding` | 0.5s | 0.8 |
| 157 | Лут: подбор XP (маленький) | `sfx_pickup_xp_small_01` | `small XP orb pickup with soft sparkle, minor experience collect, gentle ping` | 0.3s | 0.7 |
| 158 | Лут: подбор XP (средний) | `sfx_pickup_xp_med_01` | `medium XP pickup with pleasant chime, blue orb collect, rewarding ding` | 0.5s | 0.7 |
| 159 | Лут: подбор XP (большой) | `sfx_pickup_xp_large_01` | `large XP pickup with ascending magical chime, big experience reward, power gain` | 1.0s | 0.7 |
| 160 | Лут: магнит (притягивание) | `sfx_magnet_pull_01` | `magnetic pull activating with electromagnetic hum, items sucking in, force field` | 1.5s | 0.6 |
| 161 | Лут: редкий дроп | `sfx_pickup_rare_01` | `rare item dropping with shimmering sparkle, epic loot ping, golden glow, valuable` | 1.5s | 0.7 |
| 162 | Лут: подбор редкого | `sfx_pickup_rare_grab_01` | `rare item pickup with ascending triumphant chime, epic collect fanfare, reward` | 1.5s | 0.7 |
| 163 | Лут: подбор перо (гусь) | `sfx_pickup_feather_01` | `feather pickup with soft plume rustle, light item collect, airy swoosh` | 0.5s | 0.6 |
| 164 | Лут: подбор шерсть | `sfx_pickup_wool_01` | `wool pickup with soft fluffy squish, fleece collect, gentle compression` | 0.5s | 0.6 |
| 165 | Лут: подбор жало | `sfx_pickup_stinger_01` | `bee stinger pickup with small metallic click, sharp item collect, needle grab` | 0.3s | 0.7 |
| 166 | Лут: подбор ключ/секрет | `sfx_pickup_key_01` | `secret key pickup with mysterious chime, important item, quest object collect` | 1.0s | 0.7 |
| 167 | Лут: полное инвентаря | `sfx_inventory_full_01` | `inventory full error with dull thud and buzz, cannot collect, warning clunk` | 0.8s | 0.7 |
| 168 | Лут: золотое яйцо (редкое) | `sfx_pickup_golden_egg_01` | `golden egg pickup with magical sparkle and rich chime, legendary loot, precious` | 1.5s | 0.7 |
| 169 | Лут: дроп сундука | `sfx_chest_drop_01` | `treasure chest dropping with heavy wood thud, loot container arrival, valuable` | 1.0s | 0.8 |

---

### 4.6 Окружение и амбиент (20 звуков)

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 170 | Амбиент: русская деревня днём | `amb_village_day_01` | `Russian village daytime ambience, distant chicken clucks, gentle breeze through wooden fence, peaceful countryside` | 20s | 0.5 |
| 171 | Амбиент: русская деревня вечер | `amb_village_evening_01` | `Russian village evening ambience, crickets chirping, distant dog barking, sunset cicadas, calm dusk` | 20s | 0.5 |
| 172 | Амбиент: ночь в деревне | `amb_village_night_01` | `Russian village night ambience, owl hooting, distant wolf howl, cricket orchestra, dark eerie` | 20s | 0.5 |
| 173 | Амбиент: дождь | `amb_rain_01` | `rain falling on wooden roof and mud, Russian village rain, puddle drops, gentle shower` | 20s | 0.5 |
| 174 | Амбиент: ливень | `amb_rain_heavy_01` | `heavy rain pouring with thunder rumble, Russian countryside storm, downpour, dramatic weather` | 20s | 0.5 |
| 175 | Амбиент: ветер | `amb_wind_01` | `wind blowing through Russian village, wooden fence creaking, leaf rustle, autumn breeze` | 20s | 0.5 |
| 176 | Амбиент: колодец | `amb_well_01` | `old wooden well bucket creaking, rope lowering, deep water splash echo, village well` | 15s | 0.6 |
| 177 | Амбиент: лес | `amb_forest_01` | `Russian forest ambience, birch leaves rustling, birds chirping, pine wind, nature peace` | 20s | 0.5 |
| 178 | Амбиент: река/пруд | `amb_river_01` | `gentle stream flowing, water babbling over rocks, Russian river, peaceful brook` | 20s | 0.5 |
| 179 | Амбиент: костёр | `amb_campfire_01` | `bonfire crackling with wood popping, warm campfire, night fire, cozy flames` | 20s | 0.5 |
| 180 | Амбиент: огород утром | `amb_garden_morning_01` | `Russian garden morning, rooster distant crow, dew drops, bird songs, fresh day start` | 20s | 0.5 |
| 181 | Амбиент: ферма днём | `amb_farm_day_01` | `busy Russian farm daytime, mixed animal sounds, cow moo distant, pig snort, working farm` | 20s | 0.5 |
| 182 | Амбиент: метель/зима | `amb_blizzard_01` | `blizzard howling wind, snow sweeping, winter storm, freezing gale, harsh Russian winter` | 20s | 0.5 |
| 183 | Амбиент: туман | `amb_fog_01` | `eerie fog ambience, muffled distant sounds, mysterious mist, low visibility creep` | 20s | 0.5 |
| 184 | Амбиент: заброшенный дом | `amb_abandoned_01` | `abandoned Russian izba creaking, old wood settling, ghostly whisper, creepy empty house` | 20s | 0.4 |
| 185 | Амбиент: поле лаванды/цветов | `amb_flower_field_01` | `flower field with buzzing bees, gentle warm breeze, colorful meadow, summer peace` | 20s | 0.5 |
| 186 | Амбиент: подвал/темнота | `amb_cellar_01` | `dark cellar ambience, dripping water, rat squeaks, cold stone echo, creepy basement` | 20s | 0.4 |
| 187 | Амбиент: трава/луг | `amb_meadow_01` | `grass meadow gentle breeze, butterfly flutter, summer field, peaceful Russian steppe` | 20s | 0.5 |
| 188 | Амбиент: деревня праздник | `amb_village_fest_01` | `Russian village festival, distant accordion music, people laughing, celebration joy` | 20s | 0.4 |
| 189 | Амбиент: гроза | `amb_thunderstorm_01` | `thunderstorm with lightning crack, heavy rain, thunder rolling, dramatic village storm` | 20s | 0.5 |

---

### 4.7 Шаги и передвижение (15 звуков)

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 190 | Шаги: трава | `sfx_steps_grass_01` | `footsteps walking on grass, soft ground steps, nature walking, gentle rustle` | 1.0s | 0.7 |
| 191 | Шаги: грядка/земля | `sfx_steps_dirt_01` | `footsteps on dirt path, soft soil compaction, garden bed steps, muddy thud` | 1.0s | 0.7 |
| 192 | Шаги: деревянный мост/доски | `sfx_steps_wood_01` | `footsteps on wooden planks, old bridge creaking, board walk, rustic wood` | 1.0s | 0.7 |
| 193 | Шаги: грязь | `sfx_steps_mud_01` | `footsteps squelching in mud, wet ground suck, swamp walking, messy slosh` | 1.0s | 0.7 |
| 194 | Шаги: по лужам | `sfx_steps_puddle_01` | `footsteps splashing through puddles, water splash step, wet stomp` | 1.0s | 0.7 |
| 195 | Шаги: по снегу | `sfx_steps_snow_01` | `footsteps crunching in fresh snow, winter walking, powder compression, cold crackle` | 1.0s | 0.7 |
| 196 | Шаги: по камню | `sfx_steps_stone_01` | `footsteps on cobblestone, hard rock steps, gravel path, solid ground` | 1.0s | 0.7 |
| 197 | Бег: трава | `sfx_run_grass_01` | `running quickly on grass, fast nature footsteps, jogging rustle, hurried` | 1.0s | 0.7 |
| 198 | Бег: земля | `sfx_run_dirt_01` | `running on dirt path, rapid soil steps, fast ground running, urgent` | 1.0s | 0.7 |
| 199 | Бег: дерево | `sfx_run_wood_01` | `running on wooden boards, fast creaking planks, bridge sprint, hurried wood` | 1.0s | 0.7 |
| 200 | Прыжок | `sfx_jump_01` | `character jumping with spring whoosh, leap effort, jump takeoff` | 0.8s | 0.7 |
| 201 | Приземление | `sfx_land_01` | `character landing on ground with soft thud, jump impact, ground touch` | 0.5s | 0.7 |
| 202 | Спотыкание (грядка) | `sfx_stumble_01` | `character stumbling on garden bed, trip and recover, clumsy oops, funny` | 1.0s | 0.6 |
| 203 | Замедление (в грязи) | `sfx_slow_mud_01` | `movement slowing down in mud, stuck sucking sound, swamp deceleration, gooey` | 1.5s | 0.6 |
| 204 | Ускорение (буст) | `sfx_speed_boost_01` | `speed boost activating with wind rush, fast movement power up, sonic whoosh` | 1.5s | 0.7 |

---

### 4.8 Способности и магия (20 звуков)

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 205 | Магия: огненный шар | `sfx_fireball_01` | `fireball launching with roaring flame whoosh, blazing projectile, RPG magic` | 2.0s | 0.7 |
| 206 | Магия: ледяная стрела | `sfx_ice_bolt_01` | `ice bolt firing with freezing crystal sound, frost projectile, cold magic` | 1.5s | 0.7 |
| 207 | Магия: молния | `sfx_lightning_01` | `lightning strike with electric crack and thunder, zap blast, electric magic` | 2.0s | 0.8 |
| 208 | Магия: лечение/хил | `sfx_heal_01` | `healing spell with warm light chime, HP restore, golden glow, soothing magic` | 2.0s | 0.6 |
| 209 | Магия: щит/барьер | `sfx_shield_01` | `magic shield activating with bubble pop and hum, protective barrier, defense buff` | 1.5s | 0.7 |
| 210 | Магия: телепорт | `sfx_teleport_01` | `teleportation with sparkling dissolve, magical vanish, shimmer whoosh, poof` | 2.0s | 0.6 |
| 211 | Магия: огненный взрыв | `sfx_explosion_fire_01` | `fire explosion with boom and flame burst, RPG blast, scorching detonation` | 2.5s | 0.8 |
| 212 | Магия: ледяной взрыв | `sfx_explosion_ice_01` | `ice explosion with crystal shatter and frost burst, frozen detonation, cold blast` | 2.5s | 0.7 |
| 213 | Магия: ядовитое облако | `sfx_poison_cloud_01` | `poison gas cloud spreading with bubbling hiss, toxic vapor, acid green, corrosive` | 2.5s | 0.6 |
| 214 | Магия: бафф силы | `sfx_buff_power_01` | `power buff activating with muscle surge sound, red aura, strength increase, RPG buff` | 1.5s | 0.7 |
| 215 | Магия: бафф скорости | `sfx_buff_speed_01` | `speed buff with wind acceleration, blue streak, haste spell, swift boost` | 1.5s | 0.7 |
| 216 | Магия: бафф удачи | `sfx_buff_luck_01` | `luck buff with rainbow sparkle chime, golden clover effect, fortune blessing` | 1.5s | 0.6 |
| 217 | Магия: дебафф (слабость) | `sfx_debuff_01` | `weakness debuff with dark draining sound, purple shadow, stat decrease, curse` | 1.5s | 0.6 |
| 218 | Магия: эвакуация/бегство | `sfx_escape_01` | `emergency escape with smoke bomb pop, vanish in puff, ninja retreat, comical` | 1.5s | 0.6 |
| 219 | Магия: воскрешение | `sfx_revive_01` | `character revival with angelic chorus, respawn glow, life restore, divine magic` | 2.5s | 0.5 |
| 220 | Способность: рывок/даш | `sfx_dash_01` | `combat dash with blur whoosh, quick dodge, shadow step, fast reposition` | 1.0s | 0.7 |
| 221 | Способность: супер-удар | `sfx_ultimate_01` | `ultimate ability charging with epic buildup, power crescendo, super attack ready` | 3.0s | 0.7 |
| 222 | Способность: взрыв ультимейта | `sfx_ultimate_boom_01` | `ultimate attack explosion with massive screen shake boom, epic finisher, cinematic` | 3.0s | 0.8 |
| 223 | Способность: магнитная волна | `sfx_magnet_wave_01` | `magnetic wave pulse pulling items in, electromagnetic ring expansion, force pull` | 1.5s | 0.7 |
| 224 | Способность: огненный след | `sfx_fire_trail_01` | `flaming trail burning behind character, fire path sizzle, blazing footsteps` | 2.0s | 0.6 |

---

### 4.9 Кат-сцены и комиксы (10 звуков)

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 225 | Комикс: появление панели | `sfx_comic_panel_01` | `comic book page turning with paper rustle, panel slide in, page flip, cartoon` | 1.0s | 0.6 |
| 226 | Комикс: появление речи | `sfx_comic_speech_01` | `comic speech bubble popping up with inflate sound, dialogue appear, cartoon pop` | 0.5s | 0.6 |
| 227 | Комикс: переход между панелями | `sfx_comic_transition_01` | `comic panel transition with whoosh, scene change wipe, cartoon slide` | 1.0s | 0.6 |
| 228 | Комикс: удар/драка | `sfx_comic_punch_01` | `cartoon comic punch with exaggerated POW impact, fight bam, comic book hit` | 1.0s | 0.7 |
| 229 | Комикс: звёзды от удара | `sfx_comic_stars_01` | `cartoon stars circling head after hit, dazed birdies chirping, knockout dizzy` | 1.5s | 0.5 |
| 230 | Комикс: смех злодея | `sfx_comic_evil_laugh_01` | `cartoon villain evil laugh, muahaha, funny antagonist chuckle, comical evil` | 2.5s | 0.4 |
| 231 | Комикс: открытие комикса | `sfx_comic_open_01` | `comic book opening with magical flourish, story begin fanfare, adventure start` | 2.0s | 0.6 |
| 232 | Комикс: закрытие/финал | `sfx_comic_close_01` | `comic ending with final chord, to be continued, dramatic outro, story pause` | 2.0s | 0.6 |
| 233 | Комикс: мемная вставка | `sfx_comic_meme_01` | `meme sound effect with record scratch, funny interrupt, comedic stop, awkward` | 1.0s | 0.5 |
| 234 | Комикс: радостный финал | `sfx_comic_happy_end_01` | `happy ending with major key fanfare, celebration music sting, victory moment` | 2.5s | 0.5 |

---

### 4.10 Смерть, Game Over, победа (15 звуков)

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 235 | Герой: получение урона | `sfx_player_hurt_01` | `player taking damage with pained grunt, character hit, HP loss, hurt oof` | 0.8s | 0.7 |
| 236 | Герой: тяжёлое ранение | `sfx_player_hurt_heavy_01` | `player heavy damage with painful scream, critical hit reaction, agonizing` | 1.0s | 0.7 |
| 237 | Герой: смерть | `sfx_player_death_01` | `player character dying with dramatic final breath, game over death, tragic collapse` | 2.0s | 0.6 |
| 238 | Герой: низкое здоровье (сердцебиение) | `sfx_low_hp_01` | `low health heartbeat pounding, urgent pulse, danger warning, adrenaline thump` | 2.0s | 0.7 |
| 239 | Game Over | `sfx_game_over_01` | `game over with sad trombone and defeat sting, loser fanfare, comical fail` | 3.0s | 0.5 |
| 240 | Победа над боссом | `sfx_boss_victory_01` | `boss defeated with epic victory fanfare, triumphant chord, win celebration` | 3.0s | 0.7 |
| 241 | Убийство врага (обычное) | `sfx_enemy_kill_01` | `enemy defeated with small pop, creature death poof, cartoon vanish` | 0.8s | 0.6 |
| 242 | Убийство нескольких врагов | `sfx_multi_kill_01` | `multiple enemies defeated with combo explosion, chain kill, massacre pop` | 1.5s | 0.7 |
| 243 | Комбо x10 | `sfx_combo_10_01` | `10 combo achieved with rising chime, streak celebration, fighting game combo` | 1.0s | 0.7 |
| 244 | Комбо x50 | `sfx_combo_50_01` | `50 combo with epic escalating fanfare, huge streak, unstoppable, fighting game` | 2.0s | 0.7 |
| 245 | Комбо x100 | `sfx_combo_100_01` | `100 combo with legendary explosion celebration, godlike streak, ultimate combo` | 2.5s | 0.7 |
| 246 | Уровень пройден | `sfx_level_clear_01` | `stage cleared with victory jingle, mission complete, success music, accomplished` | 2.5s | 0.6 |
| 247 | Новый рекорд | `sfx_new_record_01` | `new high score with celebratory sparkle, personal best, achievement chime` | 2.0s | 0.7 |
| 248 | Воскрешение/продолжить | `sfx_continue_01` | `continue with revive sparkle, second chance magic, respawn hope, glowing` | 2.0s | 0.6 |
| 249 | Конец забега (результаты) | `sfx_run_end_01` | `run complete with tally sound, score counting, result screen music, summary` | 2.0s | 0.6 |

---

### 4.11 Специальные и редкие события (15 звуков)

| # | Название | Файл | Промпт | Dur | PI |
|---|----------|------|--------|-----|-----|
| 250 | Редкий дроп (легендарный) | `sfx_legendary_drop_01` | `legendary item dropping with epic golden explosion, rare loot fanfare, godlike ping` | 2.0s | 0.7 |
| 251 | Секрет найден | `sfx_secret_found_01` | `secret discovered with mysterious chime and sparkle, hidden item found, eureka` | 2.0s | 0.6 |
| 252 | Пасхалка | `sfx_easter_egg_01` | `easter egg activated with silly surprise sound, funny secret, comical reveal, meme` | 2.0s | 0.5 |
| 253 | Ачивка разблокирована | `sfx_achievement_01` | `achievement unlocked with triumphant fanfare, trophy sparkle, success celebration` | 2.5s | 0.7 |
| 254 | Левел-ап (игрока) | `sfx_level_up_01` | `character leveling up with ascending magical chime, power surge, growth sparkle` | 2.0s | 0.7 |
| 255 | Эволюция оружия | `sfx_weapon_evolve_01` | `weapon evolving with transformation explosion, upgrade flash, power evolution, epic` | 2.5s | 0.7 |
| 256 | Новая локация открыта | `sfx_area_unlock_01` | `new area unlocked with discovery fanfare, map expand, adventure continue, epic` | 2.5s | 0.6 |
| 257 | Первая кровь | `sfx_first_blood_01` | `first blood with dramatic impact sting, initial kill, combat start announcement` | 1.5s | 0.7 |
| 258 | Двойное убийство | `sfx_double_kill_01` | `double kill with escalating chime, two quick kills, combo announcement` | 1.5s | 0.7 |
| 259 | Тройное убийство | `sfx_triple_kill_01` | `triple kill with excited fanfare, three kills streak, announcer excitement` | 2.0s | 0.7 |
| 260 | Безумие (много убийств) | `sfx_killing_spree_01` | `killing spree with intense rising music, rampage announcement, unstoppable` | 2.0s | 0.7 |
| 261 | Финальный босс: появление | `sfx_final_boss_spawn_01` | `final boss dramatic entrance with epic dark music, ultimate villain arrival, cinematic` | 4.0s | 0.7 |
| 262 | Финальный босс: трансформация | `sfx_final_boss_transform_01` | `final boss phase 2 transformation with dark power surge, monstrous evolution, epic` | 3.5s | 0.7 |
| 263 | Игра пройдена | `sfx_game_complete_01` | `game completed with grand victory symphony, credits music, ultimate triumph` | 4.0s | 0.7 |
| 264 | Тайный босс найден | `sfx_secret_boss_01` | `secret boss discovered with ominous chord, hidden enemy found, mysterious reveal` | 2.5s | 0.6 |

---

## 5. Музыка и песни — список с промптами

### 5.1 Музыкальные треки (Instrumental)

| # | Название | Файл | Промпт | Длительность |
|---|----------|------|--------|-------------|
| 1 | **Главное меню** — Деревенская гармонь | `music_main_menu` | `Russian village folk music, bayan accordion melody, warm and nostalgic, slow tempo 80 BPM, acoustic traditional, pixel art game menu, cozy countryside, balalaika background, peaceful morning in Russian village, instrumental only` | 2:30 |
| 2 | **Огород (день)** — Бодрый забег | `music_garden_day` | `upbeat Russian folk combat music, fast tempo 130 BPM, energetic balalaika and accordion, action-packed survivor game, village defense, quirky and fun, driving rhythm, chiptune elements mixed with folk, pixel art battle` | 3:00 |
| 3 | **Огород (вечер)** — Закат | `music_garden_evening` | `Russian village sunset music, moderate tempo 100 BPM, warm bayan melody, golden hour nostalgia, relaxing but alert, evening ambience folk, acoustic guitar, peaceful countryside dusk, instrumental` | 2:30 |
| 4 | **Луг** — Полевые цветы | `music_meadow` | `meadow field folk music, moderate tempo 110 BPM, bright flute and accordion, open space freedom, nature adventure, Russian countryside, optimistic and airy, grassland exploration, instrumental only` | 3:00 |
| 5 | **Двор** — Хозяйство | `music_farmyard` | `busy farmyard music, tempo 120 BPM, rhythmic working song feel, accordion and percussion, active village life, animal sounds rhythm, productive energy, Russian folk dance elements, instrumental` | 2:30 |
| 6 | **Лесопилка** — Тёмный лес | `music_forest` | `dark Russian forest music, tempo 90 BPM, mysterious and eerie, low bayan drones, creepy woodwind, suspenseful exploration, Slavic folklore atmosphere, birch forest mystery, caution and wonder, instrumental` | 3:00 |
| 7 | **Подвал** — Тень | `music_cellar` | `dark cellar ambient music, tempo 70 BPM, creepy and claustrophobic, low drones, distant dripping, horror undertones, underground tension, abandoned basement, suspenseful drone, minimal instrumental` | 2:30 |
| 8 | **Босс: Петух** — Куриный король | `music_boss_petukh` | `epic boss battle music, giant rooster king, tempo 140 BPM, intense Russian folk metal, accordion shredding, dramatic drums, poultry villain theme, aggressive balalaika, comical but epic, instrumental battle` | 2:30 |
| 9 | **Босс: Утка** — Болотная гроза | `music_boss_utka` | `swamp boss music, tempo 130 BPM, slippery and unpredictable, water splashing percussion, duck villain theme, murky atmosphere, comical evil, Russian folk minor key, instrumental` | 2:30 |
| 10 | **Босс: Баран** — Рогатый гигант | `music_boss_ram` | `heavy ram boss music, tempo 120 BPM, powerful and brutal, deep drums and low brass, horned beast charging rhythm, earth-shaking percussion, aggressive folk metal, unstoppable force, instrumental` | 2:30 |
| 11 | **Супербосс: Бабка** — Ведьма-на-метле | `music_super_granny` | `witch granny boss music, tempo 135 BPM, mischievous and scary, fast bayan playing, flying broom whoosh rhythm, kitchen witch theme, comical horror, Slavic witch folklore, playful evil, instrumental` | 3:00 |
| 12 | **Супербосс: Внучка** — Шалость | `music_super_girl` | `mischievous girl boss music, tempo 150 BPM, playful and chaotic, fast xylophone, childish pranks, water pistol rhythm, cheeky and energetic, cartoon villain kid, toy orchestra, instrumental` | 2:30 |
| 13 | **Супербосс: Жучка** — Пёс-бандит | `music_super_dog` | `dog boss music, tempo 140 BPM, aggressive and wild, barking rhythm, flea circus undertone, animalistic combat, comical but threatening, stray dog gang, street fight energy, instrumental` | 2:30 |
| 14 | **Супербосс: Кошка** — Кошачья ночь | `music_super_cat` | `mysterious cat boss music, tempo 120 BPM, sneaky and elegant, pizzicato strings, midnight jazz undertone, feline grace, stalking predator, night village, Slavic noir, instrumental` | 3:00 |
| 15 | **Супербосс: Мышка** — Мышиный король | `music_super_mouse` | `tiny mouse boss music, tempo 160 BPM, fast and frantic, miniature circus feel, squeaky instruments, small but dangerous, nut orchestra, comical epic for tiny villain, playful danger, instrumental` | 2:30 |
| 16 | **Финальный босс** — Суд деревни | `music_final_boss` | `final boss ultimate battle, tempo 150 BPM, epic Russian folk orchestra, all themes combined, maximum intensity, village judgement day, accordion symphony, choir undertone, apocalyptic folk, grand finale, instrumental` | 3:30 |
| 17 | **Победа** — Деревенский герой | `music_victory` | `victory fanfare, triumphant Russian folk celebration, tempo 120 BPM, major key joy, balalaika and accordion, village heroes return, festive and proud, credit roll music, epic win, instrumental` | 2:30 |
| 18 | **Game Over** — Поражение | `music_game_over` | `game over sad music, slow tempo 60 BPM, melancholic bayan, defeated village, minor key sorrow, comical sadness, "try again" feel, lonely accordion, dusk at empty farm, instrumental` | 2:00 |
| 19 | **Кат-сцена** — История деревни | `music_cutscene` | `storytelling narrative music, tempo 80 BPM, warm and inviting, bard-like bayan, Russian fairy tale feel, once upon a time, village elders telling stories, nostalgic and wise, instrumental` | 2:30 |
| 20 | **Прокачка/мета** — Кузница | `music_meta_upgrade` | `meta-progression blacksmith music, tempo 100 BPM, working forge rhythm, hammer on anvil beat, construction and improvement, building up, accordion craft, making things better, instrumental` | 2:00 |
| 21 | **Левел-ап экран** — Выбор | `music_levelup_screen` | `level up selection music, tempo 90 BPM, anticipatory and exciting, choice making tension, what to pick, ascending chords, potential and possibilities, reward moment, instrumental` | 1:30 |
| 22 | **Комикс** — Панель за панелью | `music_comic` | `comic book panel transition music, tempo varying, playful staccato, scene changes, story unfolding, cartoon adventure, visual narrative accompaniment, light and fun, instrumental` | 2:00 |
| 23 | **Ачивка** — Поздравление | `music_achievement` | `achievement unlock short jingle, 10 seconds, triumphant sparkle, success sting, reward fanfare, quick celebration` | 0:10 |
| 24 | **Редкий дроп** — Сокровище | `music_rare_drop` | `rare item discovered, magical sparkle music, treasure found, legendary loot moment, golden glow chords, precious find, 8 seconds` | 0:08 |
| 25 | **Секрет** — Тайна | `music_secret_found` | `secret area found, mysterious discovery music, hidden thing revealed, eureka moment, wonder and curiosity, 10 seconds` | 0:10 |

### 5.2 Песни со словами (для кат-сцен, титров, пасхалок)

| # | Название | Файл | Промпт | Длительность |
|---|----------|------|--------|-------------|
| 26 | **Песня титров** — Былины нашей деревни | `song_credits` | `Russian village folk song, male deep vocals, nostalgic lyrics about countryside life, balalaika and accordion, traditional Slavic melody, warm and heartfelt, bayan solo, memories of village, tempo 90 BPM, singer-songwriter style` | 3:00 |
| 27 | **Песня бабки** — На метле | `song_granny` | `witch granny villain song, female theatrical vocals, mischievous and scary, fast Russian folk, flying on broomstick theme, comical evil, bayan accordion, tempo 140 BPM, Broadway villain style` | 2:30 |
| 28 | **Песня деда** — Не тронь мой огород | `song_ded` | `old man Ded defender song, gruff male vocals, protecting his garden, Russian folk rock, accordion power, tempo 130 BPM, brave and stubborn, "get off my lawn" energy, heroic grandpa` | 2:30 |
| 29 | **Песня петуха** — Кукареку (босса) | `song_petukh` | `rooster villain boss song, energetic male vocals, cock-a-doodle-doo theme, aggressive poultry king, Russian folk metal, tempo 150 BPM, comical epic, feathered tyrant anthem` | 2:00 |
| 30 | **Пасхалка: Песня про Жучку** | `song_easter_zhuchka` | `funny dog song, playful vocals, loyal village dog, chasing chickens, Russian folk comedy, balalaika, tempo 120 BPM, silly and heartwarming, pet anthem` | 1:30 |
| 31 | **Колыбельная (игра на паузе)** | `song_lullaby` | `Russian village lullaby, female gentle vocals, soft and soothing, bayan accompaniment, traditional Slavic cradle song, sleep and dreams, tempo 60 BPM, peaceful night` | 2:00 |
| 32 | **Пьяная песня (пасхалка в таверне)** | `song_drunk` | `drunk Russian village song, slurred male group vocals, tipsy chorus, accordion playing off-key, comical drinking song, tempo 100 BPM, funny and chaotic, tavern atmosphere` | 1:30 |
| 33 | **Финальная песня** — Семья вместе | `song_final` | `grand finale family song, all characters singing together, Russian folk celebration, victory and unity, balalaika orchestra, tempo 120 BPM, emotional and triumphant, reunion anthem, credits version` | 3:30 |

---

## 6. Библиотека готовых промптов (копировать и вставлять)

### Быстрые промпты для частых звуков:

```
--- УДАРЫ ---
sfx_axe_throw: "sharp metallic throwing axe whooshing through air, combat swing, pixel art game, impactful" [1.5s, PI 0.8]
sfx_sword_slash: "sword slashing through air with sharp metallic whoosh, blade swing, pixel combat, clean cut" [1.0s, PI 0.8]
sfx_blunt_hit: "heavy wooden club impact on flesh, blunt weapon thud, cartoon combat, squash hit" [1.0s, PI 0.9]
sfx_metal_clang: "metal hitting metal with loud clang, sword on armor, spark impact, medieval combat" [1.0s, PI 0.9]

--- ВЗРЫВЫ ---
sfx_explosion_small: "small cartoon explosion with pop and smoke poof, tiny blast, pixel game bomb" [1.5s, PI 0.8]
sfx_explosion_big: "massive explosion with booming detonation and debris, epic blast, screen shake rumble" [2.5s, PI 0.8]
sfx_fire_burst: "fire bursting with hot whoosh and crackle, flame explosion, scorching blast" [2.0s, PI 0.7]

--- ЖИВОТНЫЕ ---
sfx_chicken_cluck: "hen clucking happily, farmyard chicken vocalization, cartoon poultry, funny" [1.5s, PI 0.6]
sfx_rooster_crow: "rooster crowing loudly at dawn, classic cock-a-doodle-doo, farm morning" [2.5s, PI 0.7]
sfx_goose_honk: "goose honking aggressively, angry goose hiss-honk, territorial waterfowl, funny" [2.0s, PI 0.6]
sfx_sheep_baa: "sheep lamb bleating softly, cute farm animal, woolly baa, cartoon" [1.5s, PI 0.6]
sfx_dog_bark: "dog barking loudly, angry guard dog, territorial canine, aggressive woof" [1.5s, PI 0.7]
sfx_cat_meow: "cat meowing with mysterious tone, feline vocalization, creepy kitty, night" [1.5s, PI 0.5]
sfx_bee_buzz: "bee buzzing angrily, insect wing vibration, aggressive honeybee, annoying" [1.5s, PI 0.6]

--- UI ---
sfx_ui_click: "soft UI button click, subtle interface tap, pixel game menu select, gentle pop" [0.5s, PI 0.7]
sfx_ui_hover: "UI hover tick, gentle interface rollover sound, soft blip, menu highlight" [0.3s, PI 0.6]
sfx_ui_error: "error buzzer, cannot perform action, denied beep, wrong move buzz, error" [0.8s, PI 0.7]
sfx_ui_success: "confirmation checkmark with positive chime, success click, agree ding, pleasant" [0.5s, PI 0.7]

--- ЛУТ ---
sfx_pickup_coin: "coin pickup with bright metallic chime, gold collect sparkle, satisfying ding" [0.5s, PI 0.8]
sfx_pickup_xp: "XP orb pickup with soft sparkle, experience collect, gentle magical ping" [0.3s, PI 0.7]
sfx_level_up: "character leveling up with ascending magical chime, power surge, growth sparkle" [2.0s, PI 0.7]

--- АМБИЕНТ (loop) ---
amb_rain: "rain falling on wooden roof and mud, Russian village rain, puddle drops, gentle shower" [20s, PI 0.5, LOOP ON]
amb_wind: "wind blowing through Russian village, wooden fence creaking, leaf rustle, autumn breeze" [20s, PI 0.5, LOOP ON]
amb_day: "Russian village daytime ambience, distant chicken clucks, gentle breeze, peaceful countryside" [20s, PI 0.5, LOOP ON]
amb_night: "Russian village night ambience, owl hooting, distant wolf howl, cricket orchestra" [20s, PI 0.5, LOOP ON]
```

---

## 7. Технические советы и FAQ

### Как добиться максимального качества:

1. **Prompt Influence 0.8-1.0** — для точных звуков (удары, шаги, UI)
2. **Prompt Influence 0.3-0.5** — для креативных звуков (магия, странные существа)
3. **Всегда добавляй контекст** — `pixel art game`, `Russian village`, `cartoon style`
4. **Избегай** — "good", "nice", "cool" в промптах. Вместо: "sharp metallic impact with echo"
5. **Duration для SFX:** 0.5-2 сек. Для ambient: 20-30 сек. Для музыки: 2-3 мин.

### Частые проблемы и решения:

| Проблема | Решение |
|----------|---------|
| Звук "фальшивый", неправдоподобный | Увеличь Prompt Influence до 0.9, добавь больше деталей |
| Звук слишком длинный | Укажи точную Duration (1.0s или 0.5s) |
| Звук не похож на игровой | Добавь тег `pixel art game` или `8-bit retro` |
| Много шума/артефактов | Попробуй другой вариант из 4 или перегенерируй |
| Слишком реалистично (нужно cartoon) | Добавь `cartoon style`, `exaggerated`, `funny` |
| Не подходит для loop | Включи Looping параметр и генерируй 20-30 сек |

### Пример рабочей сессии (копировать в чат FeralZombie):

```
Привет! Сегодня генерируем звуки оружия для "Былины и Мемы".

Заходи: https://elevenlabs.io/app/sound-effects

Настройки:
- Duration: 1.5 секунды
- Looping: OFF
- Prompt Influence: 0.8

Промпт:
"sharp metallic throwing axe whooshing through air, combat swing, pixel art game, impactful"

Нажимай Generate. Из 4 вариантов выбирай лучший, скачивай в WAV.
Файл называй: sfx_axe_throw_01.wav
```

### Контрольный чек-лист перед генерацией:

- [ ] Промпт на английском?
- [ ] Есть Subject + Action + Scene + Quality?
- [ ] Duration установлен (не Auto)?
- [ ] Looping правильно настроен?
- [ ] Prompt Influence подобран под тип звука?
- [ ] Название файла придумано заранее?
- [ ] Хватает кредитов? (проверь Usage)

### Расход кредитов на проект (примерный):

| Этап | Звуков | Кредитов |
|------|--------|----------|
| MVP (основные SFX) | ~80 | ~16 000 |
| MVP (музыка, 5 треков) | ~5 | ~15 000 |
| Полировка (доп. SFX) | ~100 | ~20 000 |
| Полировка (доп. музыка) | ~10 | ~30 000 |
| Пасхалки и редкие | ~20 | ~4 000 |
| **ИТОГО** | **~255 SFX + ~15 треков** | **~85 000** |
| **Резерв** | — | **45 000** |

---

*Документ составлен на основе исследования ElevenLabs API и GDD игры "Былины и Мемы".*
*Версия 1.0 — 24 мая 2026*
