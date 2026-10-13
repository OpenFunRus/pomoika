# Promts.md — промпты ElevenLabs для всех звуков и музыки Vintage Story

> Промпты даны **на английском** (модель лучше понимает английский), пояснения — по-русски.
> Формат записи: `путь/имя (без .ogg)` — что положить в игру. Для **саунд-сетов** (несколько файлов, напр. `walk/grass1..3`) даю **несколько промптов** — по одному на файл; можно использовать и один промпт 3–5 раз (вариации).
> Параметры: для одиночных звуков — `duration` 0.3–1.5с, `prompt_influence` ~0.5; для амбиента/погоды/пещер — 20–30с + `loop=true`. Музыка — `force_instrumental`, 90–180с (пещерные — loop).

---

# ЧАСТЬ A. Звуки (SFX)

## A1. Блоки — `survival/sounds/block/`

### Двери/ящики/контейнеры
| Файл | Промпт (3–5) |
|------|--------------|
| `block/door` | 1) `wooden door creaking open slowly, one-shot, dry timber, foley` · 2) `heavy wooden trapdoor swinging open, creak, indoors, one-shot` · 3) `creaky wooden door latch, opening, close range foley` |
| `block/largedoor-open` | 1) `large heavy wooden door opening, deep creak, timber, one-shot` · 2) `big barn-style wooden door swinging, groaning hinges, one-shot` |
| `block/largedoor-close` | 1) `large heavy wooden door slamming shut, deep thud, one-shot` · 2) `big wooden door closing with a heavy thump, timber` |
| `block/chestopen` | 1) `wooden chest lid opening, light creak, foley, one-shot` · 2) `small wooden crate opening, hinge creak` |
| `block/chestclose` | 1) `wooden chest lid closing, soft creak thud, one-shot` · 2) `wooden crate shutting, gentle knock` |
| `block/largechestopen` | 1) `large wooden chest opening, deeper creak, one-shot` · 2) `big storage chest lid lifting, timber hinge` |
| `block/largechestclose` | 1) `large wooden chest closing, low thud, one-shot` |
| `block/barrel` | 1) `wooden barrel rolling on stone, one-shot` · 2) `empty wooden barrel tipped over, clunk` |
| `block/barrelopen` | 1) `wooden barrel lid popping open, cork release, one-shot` · 2) `barrel top unsealed, small pop` |
| `block/barrelclose` | 1) `wooden barrel lid capping shut, thud, one-shot` |
| `block/basketopen` | 1) `woven basket lifted open, light brush, foley, one-shot` · 2) `wicker basket creaking open` |
| `block/basketclose` | 1) `woven basket closing, soft brush, one-shot` |
| `block/vesselopen` | 1) `ceramic vessel lid opening, light clink, one-shot` |
| `block/vesselclose` | 1) `ceramic vessel lid closing, soft clink, one-shot` |
| `block/hopperopen` | 1) `wooden hopper door opening, dry timber, one-shot` |
| `block/hoppertumble` | 1) `wooden blocks tumbling through a chute, rolling clatter, one-shot` |
| `block/cokeovendoor-open` | 1) `heavy iron oven door creaking open, heat, one-shot` · 2) `metal kiln door swinging, groan` |
| `block/cokeovendoor-close` | 1) `heavy iron oven door closing, metallic clank, one-shot` |
| `block/metaldoor` | 1) `metal door opening, hollow clang, one-shot` · 2) `iron gate sliding open, metallic grind` |
| `block/metaldoor-place` | 1) `metal door placed, solid clang, one-shot` |
| `block/hewnfancegate` | 1) `wooden fence gate swinging, creak, one-shot` |
| `block/chandelier-break` | 1) `chandelier shattering, glass and metal falling, crash, one-shot` |
| `block/chandelier-hit` | 1) `chandelier struck, glass tinkling, metal ring, one-shot` |
| `block/pump` | 1) `old wooden water pump handle, creaking up and down, one-shot, foley` · 2) `pump well handle, rattling chains, water` |
| `block/quern` | 1) `stone quern grinding, slow rotary grind, one-shot, foley` |
| `block/leafy-picking` | 1) `picking leaves from a branch, soft rustle, foley, one-shot` |
| `block/reedtrapshake1` | 1) `bamboo reed trap shaking, rattling reeds, one-shot` · 2) `reed trap rattling, light shake` · 3) `dried reeds clattering, trap shaken` |
| `block/reedtrapshut` | 1) `reed trap snapping shut, quick rattle, one-shot` |
| `block/teleporter` | 1) `spatial teleporter powering, humming energy, sci-fi one-shot` · 2) `dimensional shift portal activation, rising hum, whoosh` |
| `block/riftward` | 1) `otherworldly rift ward humming, eerie energy, one-shot` |
| `block/torch` | 1) `torch flame flickering, soft crackle, ambient, loop` · 2) `held torch, gentle fire, looping` |
| `block/pumpkin` | 1) `carved pumpkin thumped, hollow thud, one-shot` |

### Материалы (ломать/бить/ставить) — саунд-сеты
| Файл | Промпт (3–5) |
|------|--------------|
| `block/dirt1..4` | 1) `dry dirt crumble, breaking soft earth, one-shot foley` · 2) `loose soil crumbling, granular crackle` · 3) `earthen block breaking, dust, thud` · 4) `dirt crumbling, soft granular crunch` |
| `block/chop1..3` | 1) `axe chopping into wood, sharp impact, foley one-shot` · 2) `axe striking wood, thock, impact` · 3) `wood chopping hit, solid thud` |
| `block/charcoal1..3` | 1) `crumbling charcoal, brittle granular crackle, one-shot` · 2) `charcoal breaking, fine powder dust` · 3) `soft crumbly charcoal snap` |
| `block/loosestone1..4` | 1) `loose stones tumbling, gravel rolling, one-shot` · 2) `pebbles clattering on stone` · 3) `granite rubble shifting` · 4) `loose rock tumbling, granular` |
| `block/woodcreak_1..4` (и `block/creak/`) | 1) `wooden beam creaking, slow groan, one-shot` · 2) `old timber groaning under stress` · 3) `wooden plank creak, low groan` · 4) `creaking wooden structure, dry timber` |
| `block/creak/woodcreak_long1..3` | 1) `long slow wooden creak, groaning timber, loop, tension` · 2) `deep creaking beam, sustained` · 3) `creaking wood, ominous, slow, loop` |
| `block/glass` | 1) `glass shattering, sharp break, one-shot, foley` · 2) `glass pane cracking, tinkling shards` |
| `block/ceramicbreak` | 1) `ceramic pot shattering, brittle break, one-shot` · 2) `clay pot cracking, granular ceramic` |
| `block/ceramichit` | 1) `ceramic pot struck, hollow clink, one-shot` · 2) `clay vessel hit, light crack` |
| `block/ceramicplace` | 1) `ceramic pot placed, soft set-down, one-shot` |
| `block/heavymetal-hit` / `-hit2` | 1) `heavy metal struck, deep clang, one-shot, impact` · 2) `iron block hit, resonant metallic ring` |
| `block/anvil1..3` | 1) `metal anvil struck, bright ring, one-shot, impact` · 2) `hammer on anvil, sharp ping` · 3) `anvil clank, resonant` |
| `block/meteoriciron-hit-pickaxe` / `0` | 1) `pickaxe striking dense iron ore, metallic clang, one-shot` · 2) `mining iron, hard metallic impact` |
| `block/rock-break-pickaxe` | 1) `pickaxe breaking rock, stone crack, impact one-shot` |
| `block/rock-hit-pickaxe` | 1) `pickaxe hitting rock, stone tap, one-shot` |
| `block/ingot` | 1) `metal ingot dropped, bright clink, one-shot` |
| `block/planks` | 1) `wooden plank placed, solid knock, one-shot foley` · 2) `timber block set down, thock` · 3) `wood plank placed, dry timber` |
| `block/wood-tool` | 1) `wooden tool struck, hollow knock, one-shot` |
| `block/leather` | 1) `leather struck, soft muffled hit, one-shot foley` |
| `block/cloth` | 1) `cloth struck, soft swish, one-shot foley` |
| `block/plate` | 1) `metal plate struck, dull clang, one-shot` |
| `block/vinyl` | 1) `flexible vinyl struck, soft thump, one-shot` |
| `block/loosestick` | 1) `loose sticks rattling, dry twigs, one-shot` |
| `block/stickbreak` | 1) `wooden stick snapping, dry crack, one-shot` |
| `block/stickhit` | 1) `stick struck, light knock, one-shot` |
| `block/stickplace` | 1) `stick placed, soft set, one-shot` |
| `block/gravel` | 1) `gravel shifting, granular crunch, one-shot` |
| `block/sand` | 1) `sand crumbling, granular, soft, one-shot` |
| `block/snow` | 1) `snow crunching, soft granular crunch, one-shot` |
| `block/ice` | 1) `ice cracking, brittle snap, one-shot` · 2) `frozen ice block breaking, crystalline crack` |
| `block/heavyice` | 1) `thick heavy ice cracking, deep brittle crack, one-shot` |
| `block/lava` | 1) `lava bubbling, molten liquid, sizzling, loop, ambience` |
| `block/water` | 1) `water being struck, soft splash, one-shot` |
| `block/chute` | 1) `item falling down a wooden chute, rolling clatter, one-shot` |
| `block/plant` | 1) `plant swayed, soft leaf rustle, one-shot` |

---

## A2. Шаги — `survival/sounds/walk/` и `game/sounds/walk/`

Все — **foley footsteps**, 1 шаг (0.4–0.6с), `one-shot`. Генерируй 3–4 разных на поверхность.
| Файл | Промпт (3–5) |
|------|--------------|
| `walk/grass1..3` | 1) `foley footsteps on wet grass, soft crunching, one-shot` · 2) `footsteps on dry grass, light brushing` · 3) `single step on short grass, soft` |
| `walk/stone1..3` | 1) `foley footsteps on stone, hard tap, one-shot` · 2) `boot step on cobblestone` · 3) `footstep on rock, sharp click` |
| `walk/wood1..3` | 1) `foley footsteps on wooden planks, hollow thock, one-shot` · 2) `footstep on timber floor` · 3) `boot step on wood deck` |
| `walk/ice1..4` | 1) `foley footsteps on thin ice, sharp crackle, one-shot` · 2) `step on frozen ice, crystalline` · 3) `footstep on slick ice, slight skid` · 4) `ice crunch, brittle step` |
| `walk/snow1..3` | 1) `foley footsteps in fresh snow, soft squish, one-shot` · 2) `step in snow, powdery crunch` · 3) `footstep in light snow` |
| `walk/deepsnow1..3` | 1) `footsteps in deep snow, heavy muffled squish, one-shot` · 2) `step sinking into deep snow, thick` · 3) `deep snow crunch, slow` |
| `walk/sand1..3` | 1) `foley footsteps in sand, granular shifting, one-shot` · 2) `step in soft sand, rustling` · 3) `footstep on dry sand` |
| `walk/gravel1..3` | 1) `foley footsteps on gravel, gritty crunch, one-shot` · 2) `step on loose pebbles` · 3) `gravel crunch under boot` |
| `walk/water1..2` | 1) `foley footsteps in shallow water, soft splashes, one-shot` · 2) `walking in ankle-deep water, sloshing` |
| `walk/glass1..3` | 1) `foley footsteps on glass, sharp high tap, one-shot` · 2) `step on glass floor, ringing` · 3) `footstep on glass, brittle click` |
| `walk/lava` | 1) `stepping in molten lava, sizzling, one-shot, impact` |
| `walk/sludge1..3` | 1) `foley footsteps in thick mud, heavy squelch, one-shot` · 2) `step in sludge, wet ooze` · 3) `muddy footstep, sticky` |
| `walk/cloth` | 1) `footstep, cloth shoe, soft muted, one-shot` |
| `walk/default1..4` (game) | 1) `generic foley footstep, neutral surface, one-shot` · 2) `plain step, soft` · 3) `footstep, dry, light` · 4) `single step, neutral` |
| `walk/inside/leafy/bushrustle1..5` | 1) `brushing through leafy bushes, rustling leaves, one-shot` · 2) `moving through foliage, leaf rustle` · 3) `shrubbery brushed, dry leaves` · 4) `bush rustle, soft` · 5) `leaves rustling under step` |

---

## A3. Существа — `survival/sounds/creature/`

### Общие (без вида)
| Файл | Промпт |
|------|--------|
| `creature/animal-eat1..2` / `small` | 1) `small animal eating, crunching nibbles, one-shot` · 2) `animal chewing, soft munching` · 3) (small) `tiny animal nibbling, faint crunch` |
| `creature/strawdummy-hit` | 1) `straw dummy struck, dry muffled thud, one-shot` |
| `creature/beehive` | 1) `beehive, buzzing swarm, agitated, loop, ambience` |
| `creature/beehive-wild` | 1) `wild beehive, angry buzzing, dense swarm, loop` |
| `creature/beemob` | 1) `single angry bee, buzzing, one-shot` · 2) `bee buzzing, close, one-shot` |
| `creature/beesting` | 1) `bee stinging, sharp buzz, one-shot, quick` |
| `creature/cicada` | 1) `cicada calling, bright buzzing chirp, one-shot` · 2) `cicada buzz, loud, one-shot` |
| `creature/cicada-short-looping` | 1) `cicada, short rhythmic buzz, loop, ambience` |
| `creature/coqui` | 1) `tree frog (coqui) calling, rhythmic chirp, one-shot, nighttime` |
| `creature/grasshopper` | 1) `grasshopper chirping, quick insect tick, one-shot` |
| `creature/hare-idle` | 1) `small rabbit, faint nibbling and rustling, one-shot` |
| `creature/hare-hurt` | 1) `small rabbit flinching, soft squeak, one-shot` |

### Дрейфер (дрейф/бес) — `creature/drifter-*`
| Файл | Промпт (2–4) |
|------|--------------|
| `drifter-idle1..4` | 1) `ethereal wraith, faint whispering drone, one-shot, horror, ambient` · 2) `ghostly moan, distant, eerie` · 3) `spectral whisper, unsettling` · 4) `wraith hum, cold air, dread` |
| `drifter-aggro1..2` | 1) `wraith shriek, aggressive, horror, one-shot` · 2) `eerie wailing sound, angry, rising` |
| `drifter-hit` | 1) `wraith struck, ghostly thud, one-shot` |
| `drifter-hurt` | 1) `wraith hurt, pained wail, one-shot` |
| `drifter-death` | 1) `wraith dissipating, fading whoosh, one-shot, horror` |

### Медведь — `creature/bear/`
| Файл | Промпт |
|------|--------|
| `bear/growl1..2` | 1) `bear growling, deep low snarl, one-shot, aggressive` · 2) `bear low rumbling growl, menacing` |
| `bear/attack` | 1) `bear lunging attack, heavy charge, impact, one-shot, aggressive` |
| `bear/flee` | 1) `bear retreating, heavy footsteps, one-shot` |
| `bear/hurt` | 1) `bear hurt, snarling roar, one-shot` |

### Курица — `creature/chicken/`
| Файл | Промпт |
|------|--------|
| `chicken/chick1..3` | 1) `baby chick peeping, small chirp, one-shot` · 2) `chick peep, high, faint` · 3) `small chick call` |
| `chicken/hen-idle1..4` | 1) `hen clucking, soft, one-shot` · 2) `chicken cluck, low, idle` · 3) `hen pecking, light cluck` · 4) `chicken, content clucking` |
| `chicken/hen-lay1..2` | 1) `hen clucking after laying egg, alert, one-shot` · 2) `chicken, egg-lay cluck` |
| `chicken/hen-flee` | 1) `chicken running away, flapping, quick clucks, one-shot` |
| `chicken/hurt` | 1) `chicken hurt, distressed cluck, one-shot` |
| `chicken/rooster-call` | 1) `rooster crowing, morning, one-shot` |
| `chicken/rooster-alarm1..2` | 1) `rooster alarm crow, sharp, one-shot` · 2) `rooster startled crow` |

### Коза — `creature/goat/`
| Файл | Промпт |
|------|--------|
| `goat/bleat1..4` | 1) `goat bleating, bray, one-shot` · 2) `goat bleat, nasal, one-shot` · 3) `goat bleat, low` · 4) `goat bray, sharp` |
| `goat/bleatweird` | 1) `goat, strange distorted bleat, eerie, one-shot` |
| `goat/death1..3` | 1) `goat dying, weak bleat, fading, one-shot` · 2) `goat, last bleat, soft` |
| `goat/hurt1..3` | 1) `goat hurt, distressed bleat, one-shot` · 2) `goat pain bleat` |
| `goat/goatkidbleat1..3` | 1) `baby goat kid bleat, high, one-shot` · 2) `kid goat bleat, small` |
| `goat/goatkidhurt1..3` | 1) `kid goat hurt, high distressed bleat, one-shot` |

### Волк — `creature/wolf/`
| Файл | Промпт |
|------|--------|
| `wolf/howl1..3` | 1) `wolf howling, lonely, one-shot, atmospheric` · 2) `wolf howl, long, wild` · 3) `wolf howl, distant` |
| `wolf/growl` | 1) `wolf growling, low aggressive snarl, one-shot` |
| `wolf/attack` | 1) `wolf lunging, snarl, impact, one-shot, aggressive` |
| `wolf/hurt` | 1) `wolf hurt, pained yelp, one-shot` |
| `wolf/pup-bark` | 1) `baby wolf pup, small bark, one-shot` |
| `wolf/pup-howl1..2` | 1) `pup wolf howl, high, one-shot` · 2) `young wolf howl, faint` |
| `wolf/pup-flop` | 1) `pup wolf flopping, light thud, one-shot` |
| `wolf/pup-hurt` | 1) `pup wolf hurt, small yelp, one-shot` |

### Лиса — `creature/fox/`
| Файл | Промпт |
|------|--------|
| `fox/yip` | 1) `fox yipping, high short bark, one-shot` |
| `fox/growl` | 1) `fox growling, low aggressive, one-shot` |
| `fox/attack` | 1) `fox attacking, quick snap, one-shot` |
| `fox/hurt` | 1) `fox hurt, yelp, one-shot` |
| `fox/die` | 1) `fox dying, weak yip, fading, one-shot` |

### Барсук — `creature/raccoon/`
| Файл | Промпт |
|------|--------|
| `raccoon/idle` | 1) `raccoon, light rustling and chirping, one-shot` |
| `raccoon/aggro` | 1) `raccoon agitated, hissing, one-shot, aggressive` |
| `raccoon/hurt` | 1) `raccoon hurt, sharp chirp, one-shot` |
| `raccoon/death` | 1) `raccoon dying, weak sound, one-shot` |
| `raccoon/pup-idle` | 1) `baby raccoon, faint chirping, one-shot` |
| `raccoon/pup-hurt` | 1) `baby raccoon hurt, small chirp, one-shot` |
| `raccoon/pup-death` | 1) `baby raccoon dying, faint, one-shot` |

### Свинья — `creature/pig/`
| Файл | Промпт |
|------|--------|
| `pig/idle` | 1) `pig oinking, content, one-shot` |
| `pig/attack` | 1) `pig aggressive oink, charging, one-shot` |
| `pig/hurt` | 1) `pig hurt, squealing oink, one-shot` |
| `pig/piglet-idle` | 1) `baby piglet, small oink, one-shot` |
| `pig/piglet-hurt` | 1) `baby piglet hurt, squeal, one-shot` |

### Шивер (Shiver) — `creature/shiver/`
| Файл | Промпт |
|------|--------|
| `shiver/idle1..4` | 1) `hollow wooden construct, creaking, eerie, one-shot, horror` · 2) `creepy puppet, wooden joints creaking` · 3) `hollow figure, rattling wood` · 4) `ominous wooden creak, unsettling` |
| `shiver/aggro` | 1) `creepy wooden creature, aggressive creak, one-shot, horror` |
| `shiver/hurt` | 1) `wooden puppet struck, splintering, one-shot` |
| `shiver/death` | 1) `wooden puppet collapsing, cracking and falling, one-shot` |
| `shiver/shock` | 1) `startled wooden creak, sharp, one-shot` |
| `shiver/thump1..3` | 1) `heavy wooden thump, one-shot, impact` · 2) `creepy wooden footstep, heavy` · 3) `wooden body thud` |

### Гиена — `creature/hyena/`
| Файл | Промпт |
|------|--------|
| `hyena/laugh` | 1) `hyena laughing, cackling, one-shot, eerie` |
| `hyena/growl` | 1) `hyena growling, low aggressive, one-shot` |
| `hyena/attack` | 1) `hyena lunging, snarl, one-shot, aggressive` |
| `hyena/hurt` | 1) `hyena hurt, snarling, one-shot` |
| `hyena/death` | 1) `hyena dying, weak snarl, one-shot` |

### Эйдолон — `creature/eidolon/`
| Файл | Промпт |
|------|--------|
| `eidolon/awake` | 1) `colossal stone creature awakening, deep rumble, one-shot, epic, braam` |
| `eidolon/awaken` | 1) `giant eidolon fully awake, earth-shaking growl, one-shot, braam` |
| `eidolon/death` | 1) `giant stone creature collapsing, massive crash, one-shot, braam` |
| `eidolon/hit` | 1) `stone creature struck, heavy rock thud, one-shot` |
| `eidolon/rockfallslam` | 1) `massive rock slam, heavy impact, one-shot, braam` |
| `eidolon/throw` | 1) `giant creature hurling rock, heavy whoosh, one-shot` |

### Эрел — `creature/erel/`
| Файл | Промпт |
|------|--------|
| `erel/alive` | 1) `mythical fire creature, low rumbling, one-shot, epic` |
| `erel/annoyed` | 1) `fire creature, irritated growl, one-shot` |
| `erel/call1..2` | 1) `fire creature calling, deep resonant, one-shot` · 2) `mythical beast call, distant` |
| `erel/fire` | 1) `fire creature exhaling flame, roaring fire, one-shot` |
| `erel/flap1..3` | 1) `large wing flapping, heavy whoosh, one-shot` · 2) `fire creature wing flap` · 3) `wing beat, deep` |
| `erel/glide` | 1) `creature gliding, soft wing air, loop, one-shot` |
| `erel/hurt` | 1) `fire creature hurt, pained roar, one-shot` |

### Саранча — `creature/locust/`
| Файл | Промпт |
|------|--------|
| `locust/idle` | 1) `locust, faint chirping, one-shot` |
| `locust/saw` | 1) `locust chewing, dry sawing crunch, one-shot` |
| `locust/hurt` | 1) `locust swat, dry pop, one-shot` |
| `locust/death` | 1) `locust squashed, dry pop, one-shot` |

### Колокольчик (Bell) — `creature/bell/`
| Файл | Промпт |
|------|--------|
| `bell/bell` | 1) `bell ringing, bright chime, one-shot` |
| `bell/alarm` | 1) `alarm bell, urgent ringing, one-shot` |
| `bell/listen` | 1) `bell, attentive tinkle, one-shot` |
| `bell/walk` | 1) `bell, light jingle, one-shot` |
| `bell/hurt` | 1) `bell struck, off-key clang, one-shot` |
| `bell/death` | 1) `bell broken, dull clang, one-shot` |

### Bowtorn — `creature/bowtorn/`
| Файл | Промпт |
|------|--------|
| `bowtorn/idle` | 1) `creepy bow creature, faint rustle, one-shot, horror` |
| `bowtorn/draw` | 1) `bow being drawn, tense string, one-shot` |
| `bowtorn/release` | 1) `bow release, sharp string snap, one-shot` |
| `bowtorn/reload` | 1) `bow reloading, quiet draw, one-shot` |
| `bowtorn/hurt` | 1) `creepy creature hurt, one-shot, horror` |
| `bowtorn/death` | 1) `creepy creature dying, one-shot, horror` |

### Копытные — `creature/hooved/*`
| Файл | Промпт |
|------|--------|
| `hooved/generic/call1..2` | 1) `deer, soft bleating call, one-shot` · 2) `herbivore, gentle call` |
| `hooved/generic/sniff` | 1) `deer sniffing, light breath, one-shot` |
| `hooved/medium/deer-call1..3` | 1) `medium deer, bleating, one-shot` · 2) `deer call, alert` · 3) `deer, soft bleat` |
| `hooved/medium/buck-bellow1..3` | 1) `buck bellowing, nasal low bleat, one-shot` · 2) `male deer bellow` · 3) `buck, grunting bellow` |
| `hooved/small/callsmall1..3` | 1) `small deer, high bleat, one-shot` · 2) `young deer call, soft` · 3) `small deer, frightened bleat` |
| `hooved/small/smallscream1..2` | 1) `small deer screaming, high distressed, one-shot` · 2) `fawn, frightened scream` |
| `hooved/large/elk/bugle1..2` | 1) `elk bugling, loud resonant bugle, one-shot` · 2) `male elk bugle, distant` |
| `hooved/large/elk/bellow1..2` | 1) `elk bellowing, deep, one-shot` · 2) `elk, low bellow` |
| `hooved/large/elk/bellowafter` | 1) `elk bellow, fading tail, one-shot` |
| `hooved/large/redstag/roar1..3` | 1) `red stag roaring, aggressive, one-shot` · 2) `stag, bellowing roar` · 3) `male stag, dominant roar` |
| `hooved/large/redstag/bellow1..2` | 1) `red stag bellow, deep, one-shot` · 2) `stag bellow, resonant` |
| `hooved/small/fawn/fawn1..2` | 1) `fawn, high bleat, one-shot` · 2) `baby deer, faint call` |
| `hooved/small/strange/mew1..3` | 1) `unusual creature, cat-like mew, eerie, one-shot` · 2) `strange small creature, mewling` · 3) `otherworldly small mew, unsettling` |

---

## A4. Эффекты — `survival/sounds/effect/`
| Файл | Промпт |
|------|--------|
| `effect/anvilhit1..3` | 1) `hammer striking anvil, sharp ping, one-shot` · 2) `forge hammer on anvil, ringing` · 3) `anvil hit, metallic clang` |
| `effect/anvilmergehit` | 1) `metal merging on anvil, ringing clang, one-shot` |
| `effect/cashregister` | 1) `old cash register, clattering, one-shot` |
| `effect/clayform` | 1) `clay being shaped, soft squish, one-shot` |
| `effect/clothrip` | 1) `cloth tearing, rip, one-shot, foley` |
| `effect/cooking` | 1) `food sizzling on a cookfire, bubbling, loop, ambience` |
| `effect/crusher-impact1..3` | 1) `heavy stone crusher impact, deep thud, one-shot, braam` · 2) `crushing press, heavy slam` · 3) `rock crusher, deep impact` |
| `effect/deepbell` | 1) `deep bell, low resonant, one-shot, atmospheric` |
| `effect/echochamber1..2` | 1) `echo chamber, reverberant ping, one-shot, atmospheric` · 2) `cave echo, resonant` |
| `effect/embers` | 1) `embers crackling, soft fire, loop, ambience` |
| `effect/extinguish1..2` | 1) `fire extinguished, hissing steam, one-shot` · 2) `flames doused, whoosh of air` |
| `effect/fuse` | 1) `fuse burning, crackling, one-shot, tense` |
| `effect/longfuse` | 1) `long fuse burning, slow crackle, loop, tense, ambience` |
| `effect/gearbox_turn` | 1) `gearbox turning, mechanical grind, one-shot` |
| `effect/gears` | 1) `gears meshing, mechanical clicking, loop, ambience` |
| `effect/gliding` | 1) `gliding through air, whoosh, one-shot` |
| `effect/largeexplosion` | 1) `large explosion, deep boom, one-shot, braam, impact` |
| `effect/mediumexplosion` | 1) `medium explosion, boom, one-shot, impact` |
| `effect/smallexplosion` | 1) `small explosion, pop boom, one-shot` |
| `effect/latch` | 1) `metal latch clicking shut, one-shot` |
| `effect/moltenmetal` | 1) `molten metal pouring, sizzling, loop, ambience` |
| `effect/noise` | 1) `static noise, white noise burst, one-shot, glitch` |
| `effect/planetary_gears` | 1) `planetary gears turning, complex mechanical, loop, ambience` |
| `effect/portal` | 1) `spatial portal opening, rising hum and whoosh, one-shot, sci-fi` |
| `effect/receptionbell` | 1) `reception desk bell, small ring, one-shot` |
| `effect/rift` | 1) `dimensional rift tearing, eerie energy, one-shot, glitch, braam` |
| `effect/rockslide` | 1) `rockslide, tumbling stones, rumble, one-shot, braam` |
| `effect/roperip` | 1) `rope snapping, sharp twang, one-shot` |
| `effect/ropestretch` | 1) `rope stretching, taut creak, one-shot` |
| `effect/squish1..2` | 1) `wet squish, soft, one-shot` · 2) `soft squelch` |
| `effect/stonecrush` | 1) `stone crushing, granular crackle, one-shot` |
| `effect/swoosh` | 1) `fast whoosh, air movement, one-shot` |
| `effect/tempstab-drain` | 1) `temperature stabilizer draining, hum fading, one-shot, sci-fi` |
| `effect/tempstab-low` | 1) `stabilizer low warning, beeping, one-shot` |
| `effect/tempstab-verylow` | 1) `stabilizer critical, rapid beeping, one-shot, tense` |
| `effect/timeswitch` | 1) `time switching, warping whoosh, one-shot, glitch, sci-fi` |
| `effect/toolbreak` | 1) `tool breaking, dry crack, one-shot` |
| `effect/translocate-active` | 1) `teleporter active, humming energy, loop, ambience, sci-fi` |
| `effect/translocate-breakdimension` | 1) `dimension breaking, shattering whoosh, one-shot, glitch, braam` |
| `effect/translocate-idle` | 1) `teleporter idle, low hum, loop, ambience` |
| `effect/treefell` | 1) `tree falling, heavy crash, impact, one-shot, braam` |
| `effect/water-fill` / `-1` / `-2` | 1) `water filling a container, pouring splash, one-shot` · 2) `water filling, splashing` · 3) `water poured, light splash` |
| `effect/watering` | 1) `watering, light splashing, one-shot` |
| `effect/watering-loop` | 1) `watering can, continuous water, loop, ambience` |
| `effect/water-pour` | 1) `water pouring, stream, one-shot` |
| `effect/woodgrind` | 1) `wood grinding, rasping, one-shot` |
| `effect/woodswitch` | 1) `wooden switch flipping, click, one-shot` |
| `effect/writing` | 1) `quill writing on paper, scratch, one-shot, foley` |

---

## A5. Окружение — `survival/sounds/environment/` (всё — **loop, ambience**)
| Файл | Промпт |
|------|--------|
| `environment/creek` | 1) `small creek flowing, water babbling, loop, ambience` |
| `environment/drip1..3` | 1) `water dripping in cave, echo, one-shot` · 2) `cave drip, single drop` · 3) `dripping water, slow, echo` |
| `environment/fire` | 1) `campfire crackling, loop, ambience` |
| `environment/fireplace` | 1) `indoor fireplace, gentle crackle, loop, ambience` |
| `environment/largesplash1..2` | 1) `large splash, heavy water, one-shot` · 2) `big splash, water impact` |
| `environment/mediumsplash` | 1) `medium splash, water, one-shot` |
| `environment/smallsplash` | 1) `small splash, light water, one-shot` |
| `environment/lava` | 1) `lava bubbling, molten, sizzling, loop, ambience` |
| `environment/rainwindow` | 1) `rain on a window, soft patter, loop, ambience` |
| `environment/underwater` | 1) `underwater ambience, muffled, bubbles, loop, ambience` |
| `environment/waterfall` | 1) `waterfall, rushing water, loop, ambience` |
| `environment/waterwaves` | 1) `gentle water waves lapping, loop, ambience` |
| `game/sounds/environment/wind` | 1) `wind blowing, open outdoors, loop, ambience` |

---

## A6. Погода — `survival/sounds/weather/`
| Файл | Промпт (loop где уместно) |
|------|--------------|
| `weather/wind-leafy` | 1) `wind through leafy trees, rustling, loop, ambience` |
| `weather/wind-leafless` | 1) `wind through bare trees, whistling, loop, ambience` |
| `weather/lightning-verynear` | 1) `thunder, very close, deep crack, one-shot, braam` |
| `weather/lightning-near` | 1) `thunder, near, loud rumble, one-shot` |
| `weather/lightning-distant` | 1) `thunder, distant, low rumble, one-shot, atmospheric` |
| `weather/lightning-nodistance` | 1) `thunder, full, rolling, one-shot` |
| `weather/lowgrumble` | 1) `low thunder grumble, rolling, loop, ambience` |
| `weather/tracks/rain-leafy` | 1) `rain on leaves, forest, loop, ambience` |
| `weather/tracks/rain-leafless` | 1) `rain on bare ground/rooftop, steady, loop, ambience` |
| `weather/tracks/hail` | 1) `hail pelting, rattling, loop, ambience` |
| `weather/tracks/lowtremble` | 1) `storm tremble, low rumble, loop, ambience` |
| `weather/tracks/verylowtremble` | 1) `very low storm rumble, distant, loop, ambience` |

---

## A7. Игрок — `game/sounds/player/` + `survival/sounds/player/`
| Файл | Промпт |
|------|--------|
| `player/build` | 1) `block placed, solid knock, one-shot, foley` |
| `player/buildhigh` | 1) `block placed, higher pitched knock, one-shot` |
| `player/collect1..3` | 1) `item pickup, soft pluck, one-shot, ui` · 2) `collect item, light click` · 3) `item acquired, soft pop` |
| `player/destruct` | 1) `block breaking, granular crumble, one-shot, impact` |
| `player/death1..2` | 1) `player dying, soft fall, one-shot` · 2) `player death, muffled thud` |
| `player/hurt1..4` | 1) `player hurt, short gasp, one-shot` · 2) `player hit, grunt` · 3) `player pain, oof` · 4) `player struck, muffled` |
| `player/drink1..2` | 1) `drinking from a cup, gulping, one-shot` · 2) `sipping drink, liquid` |
| `player/eat` | 1) `eating, chewing, one-shot, foley` |
| `player/eat_crunchy` | 1) `eating crunchy food, crunching, one-shot, foley` |
| `player/jump` | 1) `jump, small whoosh, one-shot` |
| `player/knap1..2` | 1) `bone knapping, stone striking, one-shot` · 2) `flint knapping, chipping` |
| `player/projectilehit` | 1) `projectile impact, thud, one-shot, impact` |
| `player/quickthrow` | 1) `quick throw, whoosh, one-shot` |
| `player/slap` | 1) `slap, sharp, one-shot` |
| `player/swim` | 1) `swimming, splashing, one-shot` |
| `player/throw` | 1) `throwing, whoosh, one-shot` |
| `player/clayform` / `clayformhi` | 1) `clay forming, squish, one-shot` · 2) (hi) `clay forming, higher, one-shot` |
| `survival/player/coin1..6` | 1) `coin clinking, bright, one-shot` · 2) `coin dropping, clink` · 3) `coins jingling` · 4) `coin, high ping` · 5) `coin, low clink` · 6) `coins, few, clink` |
| `survival/player/chalkdraw1..3` | 1) `chalk drawing, scratch, one-shot, foley` · 2) `chalk on stone, rasping` · 3) `chalk writing, soft` |
| `survival/player/gluerepair1..4` | 1) `glue repair, soft squish, one-shot` · 2) `gluing, sticky` · 3) `repair, soft set` · 4) `glue applied, light` |
| `survival/player/clothrepair` | 1) `cloth repairing, sewing, one-shot` |
| `survival/player/hackingspearhit` | 1) `hacking spear strike, impact, one-shot` |
| `survival/player/handdrill` | 1) `hand drill, rasping wood, one-shot` |
| `survival/player/messycraft` | 1) `messy crafting, fumbling, one-shot` |
| `survival/player/panning` | 1) `panning for gold, water swirl, one-shot` |
| `survival/player/poultice` / `-applied` | 1) `poultice applied, soft, one-shot` · 2) `poultice, gentle pat` |
| `survival/player/scrape` | 1) `scraping, rasping, one-shot` |
| `survival/player/seal` | 1) `sealing, soft press, one-shot` |
| `survival/player/squeezehoneycomb` | 1) `squeezing honeycomb, sticky squelch, one-shot` |
| `survival/player/stab` | 1) `stabbing, thrust, one-shot, impact` |
| `survival/player/strike1..2` | 1) `striking, sharp hit, one-shot` · 2) `strike, impact` |
| `survival/player/wetclothsqueeze` | 1) `squeezing wet cloth, dripping squelch, one-shot` |

---

## A8. Инструменты/ремонт — `survival/sounds/tool/`, `held/`, `wearable/`
| Файл | Промпт |
|------|--------|
| `tool/slash` | 1) `tool slashing, whoosh, one-shot` |
| `tool/scythe1..2` | 1) `scythe swinging, whoosh, one-shot` · 2) `scythe cutting, swish` |
| `tool/sling1` | 1) `sling released, whoosh, one-shot` |
| `tool/padlock` | 1) `padlock, locking click, one-shot, metallic` |
| `tool/reinforce` | 1) `reinforcing, hammering, one-shot` |
| `tool/breakreinforced` | 1) `breaking reinforced, crack, one-shot` |
| `held/bookturn1..3` | 1) `book page turning, soft whoosh, one-shot, foley` · 2) `page flip` · 3) `book page, light` |
| `held/bookclose1..3` | 1) `book closing, soft thud, one-shot` · 2) `book shut, light` |
| `held/shieldblock-wood-light` / `-heavy` | 1) `wooden shield block, light thud, one-shot` · 2) (heavy) `wooden shield block, deep` |
| `held/shieldblock-metal-light` / `-heavy` | 1) `metal shield block, light clang, one-shot` · 2) (heavy) `metal shield block, deep clang` |
| `held/torch-idle` | 1) `torch held, flame flicker, loop, ambience` |
| `held/torch-equip` | 1) `torch equipped, flame ignite, one-shot` |
| `held/torch-unequip` | 1) `torch unequipped, flame out, one-shot` |
| `held/torch-attack` | 1) `torch swing attack, whoosh, one-shot` |
| `wearable/leather1..3` | 1) `leather armor, light movement, creak, one-shot, foley` · 2) `leather, soft` · 3) `leather, swish` |
| `wearable/chain1..2` | 1) `chain armor, light jingle, one-shot, metallic` · 2) `chainmail, clinking` |
| `wearable/scale1..2` | 1) `scale armor, clinking, one-shot` · 2) `scales, light metallic` |
| `wearable/plate1..4` | 1) `plate armor, solid movement, clank, one-shot, metallic` · 2) `plate, heavy` · 3) `plate, light` · 4) `plate, clink` |
| `wearable/brigandine1..2` | 1) `brigandine armor, light clink, one-shot` · 2) `brigandine, metallic` |

---

## A9. Голоса/инструменты — `voice/`, `instrument/`
Для «одного инструмента» — ключевое слово **`solo`** + конкретный звук. Генерируй 7 «нот» (разной высоты/длины) на инструмент.
| Набор | Промпт (пример 7 нот) |
|--------|------------------------|
| `survival/sounds/voice/accordion/*` (7) | `solo accordion, low note` · `solo accordion, mid note` · `solo accordion, high note` · `solo accordion, short pluck` · `solo accordion, low long` · `solo accordion, high short` · `solo accordion, mid staccato` |
| `voice/altoflute/*` | `solo alto flute, low` / `mid` / `high` / `short` / `long low` / `high short` / `mid staccato` |
| `voice/clarinet/*` | `solo clarinet, low` / `mid` / `high` / `short` / `long` / `high short` / `staccato` |
| `voice/duduk/*` | `solo duduk, low drone` / `mid` / `high` / `short` / `long` / `high short` / `melodic` |
| `voice/harmonica/*` | `solo harmonica, low` / `mid` / `high` / `short` / `long` / `high short` / `bend` |
| `voice/harp/*` | `solo harp, low pluck` / `mid` / `high` / `short` / `long arpeggio` / `high short` / `mid` |
| `voice/harpsichord/*` | `solo harpsichord, low` / `mid` / `high` / `short` / `long` / `high short` / `staccato` |
| `voice/oboe/*` | `solo oboe, low` / `mid` / `high` / `short` / `long` / `high short` / `staccato` |
| `voice/ocarina/*` | `solo ocarina, low` / `mid` / `high` / `short` / `long` / `high short` / `melodic` |
| `voice/sax/*` | `solo saxophone, low` / `mid` / `high` / `short` / `long` / `high short` / `jazz bend` |
| `voice/trumpet/*` | `solo trumpet, low` / `mid` / `high` / `short` / `long` / `high short` / `brass` |
| `voice/tuba/*` | `solo tuba, low` / `mid` / `high` / `short` / `long` / `low short` / `deep` |
| `game/sounds/voice/*` (8) | те же шаблоны: `solo accordion` / `alto flute` / `clarinet` / `harmonica` / `oboe` / `sax` / `trumpet` / `tuba` |
| `survival/sounds/voice/saxophone` | `solo saxophone, expressive note, one-shot` |
| `survival/sounds/instrument/elkcall` | `elk call, hunting call, resonant bugle, one-shot` |

---

# ЧАСТЬ B. Музыка

> Все треки: `force_instrumental`, длительность 90–180с (для фоновых). Промпт = **жанр + настроение + инструменты + BPM + эпоха**. Не забывай **исключения** (`no vocals`, `no percussion`) для ambient.

## B1. Поверхность — день/вечер/ночь
| Файл | Промпт (2–3 варианта) |
|------|------------------------|
| `night-to-day` | 1) `gentle acoustic dawn ambient, soft guitar and warm strings, hopeful, 70 BPM, in D major, no vocals, instrumental, cinematic` · 2) `peaceful morning ambient, pluck and light pad, uplifting, 72 BPM, A major, instrumental` |
| `to-dawn` | 1) `rainy night to dawn, soft melancholic ambient, piano and pad, 65 BPM, in F minor, no vocals, instrumental` |
| `daylight` | 1) `bright daytime ambient, acoustic guitar and light percussion, warm, 80 BPM, in G major, no vocals, instrumental` · 2) `sunny daylight, folk acoustic, joyful, 82 BPM, D major, instrumental` |
| `hallowcroft` | 1) `medieval folk ambient, lute and fiddle, pastoral, 75 BPM, in A major, no vocals, instrumental` · 2) `village folk, warm acoustic, 74 BPM, E major, instrumental` |
| `setting-sun` | 1) `sunset ambient, mellow strings and soft flute, reflective, 70 BPM, in C major, no vocals, instrumental` · 2) `evening, gentle acoustic, warm, 72 BPM, G major, instrumental` |
| `creating` | 1) `creative focus ambient, light pluck and airy pads, 78 BPM, in Bb major, no vocals, instrumental` |
| `mirror` | 1) `calm introspective ambient, piano and soft strings, 68 BPM, in D minor, no vocals, instrumental` |
| `vintagestory` (тема) | 1) `signature ambient folk theme, warm strings, lute, and flute, epic but gentle, 76 BPM, in D major, no vocals, cinematic, instrumental` · 2) `nostalgic folk theme, orchestral-acoustic blend, 74 BPM, A major, instrumental` |
| `sunny-village-create` | 1) `cheerful village folk, bright acoustic, lute and fiddle, 84 BPM, in D major, no vocals, instrumental` |
| `peaceful-village` | 1) `peaceful village ambient, soft strings and flute, warm, 72 BPM, in C major, no vocals, instrumental` |
| `groove` | 1) `relaxed folk groove, acoustic guitar and light percussion, laid-back, 88 BPM, in A major, no vocals, instrumental` |
| `building` | 1) `upbeat building/work ambient, driving acoustic rhythm, motivated, 92 BPM, in G major, no vocals, instrumental` |
| `through-the-grass-survive` | 1) `night tension ambient, low strings and soft wind, uneasy, 60 BPM, in D minor, no vocals, no percussion, instrumental` · 2) `dark grassy night, sparse pluck and dread pad, 58 BPM, F minor, instrumental` |
| `spring` | 1) `springtime ambient, light flute and strings, fresh, 78 BPM, in E major, no vocals, instrumental` |
| `summer-day` | 1) `warm summer day ambient, acoustic guitar and flute, relaxed, 80 BPM, in A major, no vocals, instrumental` |
| `summer-stroll` | 1) `summer stroll, gentle folk, light and airy, 76 BPM, in D major, no vocals, instrumental` |
| `tuningcylinder/theinvention` | 1) `wondrous invention ambient, harpsichord and pluck, curious, 74 BPM, in C major, no vocals, instrumental` |
| `fall-o'-croft` | 1) `autumn ambient, mellow fiddle and strings, melancholic-warm, 72 BPM, in F major, no vocals, instrumental` |
| `fall` | 1) `autumn ambient, soft pluck and pad, reflective, 70 BPM, in D minor, no vocals, instrumental` |
| `winter` | 1) `cold winter ambient, sparse piano and airy pad, stark, 62 BPM, in C minor, no vocals, no percussion, instrumental` |
| `arcticwinds` | 1) `arctic ambient, wind textures and low drone, cold and vast, 55 BPM, in A minor, no vocals, no percussion, loop, instrumental` |
| `adventuring` | 1) `adventure ambient, hopeful strings and light percussion, 82 BPM, in D major, no vocals, instrumental` |
| `midnight` | 1) `midnight ambient, sparse and quiet, low strings and faint pluck, 55 BPM, in D minor, no vocals, no percussion, loop, instrumental` |
| `nostalgic` | 1) `nostalgic ambient, warm piano and strings, tender, 68 BPM, in E major, no vocals, instrumental` |
| `heartbeat-survive` / `-create` | 1) `low heartbeat-driven ambient, tension, slow pulse, 60 BPM, in D minor, no vocals, no melody, loop, instrumental` |
| `radianceandrust` | 1) `epic ambient, orchestral strings with subtle industrial texture, awe, 70 BPM, in D minor, no vocals, cinematic, instrumental` |
| `chilly-village` | 1) `chilly village ambient, muted strings and flute, cold, 68 BPM, in F minor, no vocals, instrumental` |
| `safety-of-a-warm-fire` | 1) `warm fireside ambient, soft strings and crackle texture, cozy, 64 BPM, in D major, no vocals, instrumental` |
| `windy-village` | 1) `windy village, airy strings and flute, movement, 74 BPM, in G major, no vocals, instrumental` |
| `sunny-village-survive` | 1) `sunny village survive, bright folk acoustic, 80 BPM, in D major, no vocals, instrumental` |
| `substitute-epitaph` | 1) `somber ambient, piano and low strings, mournful, 60 BPM, in C minor, no vocals, instrumental` |
| `the-lazaret` | 1) `melancholic ambient, sparse strings, eerie, 62 BPM, in E minor, no vocals, instrumental` |
| `tobias` | 1) `gentle ambient, warm pluck and strings, 72 BPM, in A major, no vocals, instrumental` |
| `devastation-baselayer` | 1) `devastation ambient, dark drone and low strings, ominous, 55 BPM, in D minor, no vocals, no percussion, loop, instrumental` |
| `devastation-bellsandrust` | 1) `devastation, dissonant bells and rust texture, dread, 58 BPM, in B minor, no vocals, instrumental` |
| `devastation-erelfight` | 1) `intense battle ambient, driving percussion and dark strings, 120 BPM, in D minor, no vocals, cinematic, instrumental` |
| `devastation-erelharrass` | 1) `harassment tension, sparse staccato strings and low pulse, 100 BPM, in E minor, no vocals, instrumental` |
| `game/music/roots` | 1) `roots ambient, folk acoustic, warm and grounded, 74 BPM, in D major, no vocals, instrumental` |
| `game/music/night-to-day` | 1) `gentle dawn ambient, soft acoustic, hopeful, 70 BPM, in D major, no vocals, instrumental` |
| `game/music/nostalgic` | 1) `nostalgic ambient, piano and strings, 68 BPM, in E major, no vocals, instrumental` |

## B2. Пещеры — `survival/music/deepunderground/` (всё — **loop, ambient drone, no melody/percussion**)
Генерируй как **бесшовные лупы** (см. ElevenLabs.md §5.2). Части (`parts[]` в `musicconfig.json`) группируют файлы по префиксу.
| Файл/группа | Промпт |
|------|--------------|
| `aquatic drone 1a..2b` (4) | 1) `underwater cave drone, deep aquatic hum, echo, loop, no melody, no percussion, dark ambient` · 2) (вариации — разная глубина/пульсация) |
| `bell piano 1..8` | 1) `deep underground bell-piano, sparse resonant notes, eerie, loop, no percussion, dark ambient` · 2) (разные интервалы) |
| `bells 1..2` | 1) `cave bells, distant resonant chime, loop, no melody, dark ambient, echo` |
| `deep drone 1..3` | 1) `deep cave drone, low sustained hum, dark, loop, no melody, no percussion, atmospheric` |
| `metal bass 1..3` | 1) `metallic bass drone, industrial-cave texture, low, loop, no melody, dark ambient` |
| `piece 1..9` | 1) `underground ambient piece, sparse piano and drone, evolving, loop, no percussion, dark ambient` · 2) (разные фрагменты) |
| `ticking 1..4` | 1) `cave ticking, slow rhythmic mechanical tick, sparse, loop, no melody, dark ambient, tense` |

## B3. Event — `tuningcylinder/` + resonancearchive
| Файл | Промпт |
|------|--------------|
| `tuningcylinder/culturedtavern` | 1) `tavern ambient, warm folk, lute and fiddle, 80 BPM, in G major, no vocals, instrumental` |
| `tuningcylinder/quirkytavern` | 1) `quirky tavern, playful folk, 84 BPM, in A major, no vocals, instrumental` |
| `tuningcylinder/the-seraphs` | 1) `celestial ambient, ethereal choir-pad and strings, transcendent, 66 BPM, in C major, no vocals, instrumental` |
| `tuningcylinder/theinvention` | 1) `invention ambient, curious pluck and harpsichord, 74 BPM, in C major, no vocals, instrumental` |
| `theresonancearchives-barren` | 1) `barren archive ambient, vast echoing pad, sparse, 55 BPM, in D minor, no vocals, no percussion, loop, dark ambient` |
| `theresonancearchives-eidolon` | 1) `eidolon archive, epic dark ambient, low braam and strings, 60 BPM, in D minor, no vocals, cinematic, instrumental` |
| `theresonancearchives-library` | 1) `library archive ambient, warm and reverent, strings and soft pluck, 68 BPM, in C major, no vocals, instrumental` |

## B4. Creative — `creative/music/`
| Файл | Промпт |
|------|--------------|
| `heartbeat-create` | 1) `calm heartbeat ambient, gentle pulse, 60 BPM, in D major, no vocals, no percussion, loop, instrumental` |
| `sunny-village-create` | 1) `bright creative village folk, acoustic, 80 BPM, in D major, no vocals, instrumental` |
| `through-the-grass-create` | 1) `gentle grass ambient, soft pluck and pad, peaceful, 66 BPM, in A major, no vocals, loop, instrumental` |

---

## Как пользоваться этим файлом (кратко)
1. Для каждого **набора** бери нужное число промптов = числу файлов (напр. `walk/grass` — 3 файла → 3 промпта).
2. **Одиночные** (door, fire, bear/growl) — 1–2 промпта, бери лучший из 2–3 генераций.
3. **Амбиент/погода/пещеры** — включай `loop` (SFX) или генерируй луп-музыку (см. [ElevenLabs.md](./ElevenLabs.md) §5.2).
4. Генерация → WAV/MP3 → **OGG** (ffmpeg) → путь `assets/<pack>/...` без `.ogg` → игра → чек-лист.

> **Имена файлов** в этом файле сверены с реальной папкой `survival/sounds/` (скан v1.21.5). Перед копированием в игру **ещё раз проверь точное имя** в соответствующей подпапке — кладя файл, используй **точно** то имя, что лежит в папке (без `.ogg`).
