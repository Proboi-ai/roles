# Справочник: анатомия промпта и инструменты

Рабочий справочник — таблицы, словари, примеры. Используй при сборке промптов.

## Анатомия промпта: 7 слоёв

| Слой | Что описывает | Примеры |
|---|---|---|
| **Субъект** | Кто или что главное, детали, действие | `a young woman with short red hair, smiling`, `a glass perfume bottle with golden cap`, `a snow leopard mid-leap` |
| **Среда** | Фон, обстановка, атмосфера | `in a minimalist studio`, `on a foggy mountain ridge at dawn`, `inside a cozy library with warm lighting` |
| **Стиль** | Жанр, техника, художественный референс | `oil painting`, `in the style of Studio Ghibli`, `editorial fashion photography`, `ukiyo-e woodblock print` |
| **Свет** | Источник, направление, качество, температура | `soft golden hour light from the left`, `dramatic rim lighting`, `overcast diffused daylight`, `neon glow reflecting off wet pavement` |
| **Композиция и ракурс** | Кадрирование, угол, глубина | `close-up portrait`, `bird's eye view`, `wide establishing shot`, `shallow depth of field`, `rule of thirds` |
| **Качество и детали** | Разрешение, текстура, технические уточнения | `8k ultra detailed`, `shot on Canon EOS R5 85mm f/1.4`, `hyperrealistic`, `matte texture`, `intricate details` |
| **Негативный промпт** | Что исключить | `blurry, overexposed, extra fingers, watermark, low quality, cropped` |

### Порядок слоёв в строке промпта

```
[субъект], [среда], [стиль], [свет], [композиция], [качество] --no [негативный]
```

Не все слои нужны всегда. Для простого арта достаточно субъект + стиль + свет. Для коммерческого фото — все семь.

---

## Соотношения сторон под задачу

| Задача | Соотношение | Примечание |
|---|---|---|
| Логотип / иконка | `1:1` | Квадрат, работает на всех площадках |
| Пост Instagram / VK | `1:1` или `4:5` | 4:5 заполняет больше экрана |
| Stories / Reels / Shorts | `9:16` | Вертикаль на весь экран |
| Обложка Telegram-канала | `1:1` | Аватар всегда квадратный |
| Обложка книги / лонгрид | `2:3` или `3:4` | Портретная ориентация |
| Баннер / шапка сайта | `16:9` или `21:9` | Широкий горизонт |
| Фото товара (маркетплейс) | `1:1` | Белый или нейтральный фон |
| Кинопостер / арт-принт | `2:3` | Классика постерного формата |

В Midjourney: `--ar 1:1`, `--ar 9:16` и т.д.
В DALL-E / Stable Diffusion: выбирается в настройках генерации.

---

## Словарь стилей

### Фотографические
- `editorial photography` — модная/журнальная съёмка
- `product photography on white background` — фото товара
- `documentary photography` — репортажный стиль, живой момент
- `golden hour photography` — тёплый закатный свет
- `studio portrait, soft box lighting` — классический студийный портрет
- `macro photography` — крупный план, мелкие детали
- `drone aerial shot` — вид с высоты

### Иллюстративные
- `digital illustration` — цифровая иллюстрация
- `flat design illustration` — плоский векторный стиль
- `watercolor illustration` — акварель, мягкие переходы
- `ink drawing, lineart` — чёрно-белая графика пером
- `concept art` — концепт-арт, игровая/кинематографическая эстетика
- `isometric illustration` — изометрия, техничный вид
- `comic book style` — комиксовая графика

### Художественные движения и техники
- `oil painting, impressionist` — живопись, импрессионизм
- `Art Deco poster` — ар-деко, геометрия и золото
- `Bauhaus minimalism` — функциональный минимализм
- `ukiyo-e woodblock print` — японская гравюра
- `brutalist graphic design` — брутализм, грубые шрифты и контраст
- `retrowave / synthwave` — ретро-неоновая эстетика 80-х
- `cottagecore aesthetic` — уютная деревенская идиллия

### Художественные референсы (указывай осторожно в коммерческих целях)
- `in the style of Monet` — пейзажи, мягкий свет
- `in the style of Alphonse Mucha` — ар-нуво, декоративные линии
- `Studio Ghibli aesthetic` — японская анимация, тёплая атмосфера
- `cinematic, Wes Anderson composition` — симметрия, пастельные цвета

---

## Свет: ключевые термины

| Тип света | Эффект | Когда использовать |
|---|---|---|
| `soft diffused light` | Нежные тени, ровный тон | Портрет, красота, еда |
| `golden hour light` | Тёплый оранжевый, длинные тени | Пейзаж, уличное фото |
| `blue hour light` | Холодный синий сумрак | Городская сцена, романтика |
| `dramatic side lighting` | Резкие контрасты, объём | Арт-портрет, предмет |
| `rim lighting / backlight` | Обводка по краю субъекта | Силуэт, драма |
| `neon lighting` | Яркий цветной ореол | Ночной город, киберпанк |
| `studio softbox` | Равномерный, профессиональный | Товар, портрет |
| `candlelight / firelight` | Тёплый мерцающий свет | Уют, исторический сеттинг |
| `overcast light` | Рассеянный, без теней | Пейзаж, нейтральный тон |

---

## Композиция: ключевые термины

| Приём | Описание |
|---|---|
| `rule of thirds` | Субъект смещён от центра на треть кадра |
| `centered composition` | Субъект по центру, симметрия |
| `leading lines` | Линии ведут взгляд к субъекту |
| `frame within frame` | Субъект обрамлён аркой, деревьями и т.д. |
| `negative space` | Много пустого пространства вокруг субъекта |
| `shallow depth of field` | Субъект в фокусе, фон размыт (bokeh) |
| `wide angle` | Широкий охват, искажение перспективы |
| `telephoto compression` | Длинный фокус, «сжатый» фон |
| `bird's eye view` | Вид сверху |
| `worm's eye view` | Вид снизу, субъект монументален |
| `close-up / macro` | Крупный план, детали |

---

## Негативные промпты: базовый набор

Для большинства задач подходит этот набор — добавляй или убирай по ситуации:

```
blurry, out of focus, low quality, pixelated, overexposed, underexposed,
extra limbs, extra fingers, deformed hands, watermark, signature, text,
cropped, frame cut, bad anatomy, ugly, distorted face
```

**Для товарной фотографии добавь:**
```
shadows on product, reflections, cluttered background, bent packaging
```

**Для портрета добавь:**
```
asymmetrical eyes, skin blemishes, unnatural skin tone, plastic look
```

**Для минималистичного дизайна:**
```
complex background, busy composition, overdecorated, photorealistic
```

---

## Как итерировать

1. **Получил результат, что-то не так** → определи, какой слой сломан: субъект? свет? стиль? Меняй только его.
2. **Слишком генерично** → добавь конкретики в субъект (детали одежды, цвет глаз, форма объекта).
3. **Стиль не тот** → уточни художественный референс или технику (oil painting vs watercolor vs lineart).
4. **Свет плоский** → добавь источник и направление (left side rim light, window light from above).
5. **Артефакты** → расширь негативный промпт (deformed, artifact, glitch).
6. **Нужно больше атмосферы** → добавь описание среды и атмосферные слова (misty, ethereal, moody, cinematic).

## Частые ошибки

| Ошибка | Что делать |
|---|---|
| Слишком длинный промпт (>200 слов) | Оставь самое важное, уберите повторы |
| Расплывчатые слова («красивый», «хороший») | Замени конкретными: `vibrant colors`, `elegant silhouette` |
| Противоречия в стиле | Не смешивай несовместимое: `photorealistic` + `cartoon` |
| Забыли про свет | Даже простой `soft natural light` кардинально меняет результат |
| Нет негативного промпта | Без него часто вылезают артефакты и лишние конечности |
| Соотношение сторон не задано | Укажи `--ar` или выбери в настройках под задачу |
