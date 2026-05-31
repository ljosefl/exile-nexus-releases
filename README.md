# Exile Nexus

**Единый компаньон для Path of Exile 2** — цены, фильтр, билды, стэш, кампания и «что фармить» в одном окне.

[![Latest release](https://img.shields.io/github/v/release/ljosefl/exile-nexus-releases?label=версия&sort=semver)](https://github.com/ljosefl/exile-nexus-releases/releases/latest)
![Platform](https://img.shields.io/badge/platform-Windows%20x64-blue)
![PoE2](https://img.shields.io/badge/Path%20of%20Exile-2-c24)

> Этот репозиторий — **публичный канал установщиков**. Исходный код разрабатывается отдельно; здесь только `.exe` для игроков и автообновления приложения.

---

## Скачать

1. Откройте **[Releases → Latest](https://github.com/ljosefl/exile-nexus-releases/releases/latest)**  
2. Скачайте **`Exile.Nexus_*_x64-setup.exe`**  
3. Установите и запустите **Exile Nexus**

Обновления в приложении: **Settings → Обновления** (канал уже настроен, GitHub-токен не нужен).

---

## Что умеет Exile Nexus

Один desktop-клиент вместо набора разрозненных утилит. Все модули работают через **официальные API GGG**, **буфер обмена** и **Client.txt** — без вмешательства в процесс игры.

| Модуль | Для чего | Аналог |
|--------|----------|--------|
| **Price Check** | Оценка предмета поверх игры, горячая клавиша **Alt+F** | Awakened PoE Trade |
| **Loot Filter** | Правила, пресеты, sync + **автоскан папки** `.filter` | FilterBlade |
| **Build Planner** | PoB, `.build`, **автоскан BuildPlanner**, демо отдельно | Path of Building |
| **Что фармить** | Мета-uniques, вердикты farm / watch / skip, цены trade2 | — |
| **Farm Lab** | EV фарма, стратегии, учёт валюты с пола | — |
| **Campaign** | Гайд по актам, чеклисты, виджет поверх игры | — |
| **Stash Helper** | Шаблоны табов, chaos recipe, авто-отметка слотов | Exile UI |
| **Trade** | Поиск trade2, bulk whisper, throttling запросов | trade.pathofexile.com |

### Price Check — оверлей цен

- Наведите курсор на предмет в игре → **Ctrl+C** → **Alt+F**  
- Цены с **trade2**, курсы с **poe.ninja**, компактный overlay поверх клиента  
- Отдельные **виджеты** (кампания, Farm Lab) — расставляете по экрану как удобно

### Loot Filter

- Редактор правил, пресеты под старт лиги и маппинг  
- Экспорт официального `.filter` и **авто-sync** в Documents/Path of Exile 2  
- **Автоскан папки** — скачанные FilterBlade `.filter` видны в списке; правила из `*.rules.json` подгружаются сами  
- Создание правила из предмета в буфере

### Build Planner

- Импорт **Path of Building** и `.build`  
- **4700+** имён нод дерева PoB2  
- **Автоскан папки BuildPlanner** — ваши `.build` подтягиваются с диска (обновление раз в минуту)  
- Один **демо-билд** отдельно — не мешает вашим и не пропадает после обновления  
- Экспорт в папку Build Planner клиента PoE 2  
- Ссылка на модуль **«Что фармить»** — какие uniques актуальны под мету

### Что фармить + Farm Lab

- Рейтинг uniques: популярность билдов (poe.ninja) × цена (trade2 при POESESSID)  
- Вердикты: **выгодно** / **смотреть** / **не приоритет**  
- NLP по патч-ноутам GGG и схемы фарма внутри приложения  
- **Farm Lab** — expected value стратегий, сессии, учёт дропа с Client.txt

### Campaign

- Пошаговый гайд кампании PoE2, прогресс по актам  
- Виджет и мини-map checker в overlay  
- Сброс прогресса, таймер, синхронизация между вкладками

### Stash Helper

- Шаблоны организации табов  
- **Chaos recipe**: подсказки по слотам, авто-отметка при Alt+F  
- Классификация предмета из буфера

---

## Быстрый старт

```text
1. Settings  → лига, POESESSID («Найти на ПК» после входа на pathofexile.com/trade2)
2. Dashboard → «Пресет старта лиги» (кампания, рынок, stash, цены, фильтр)
3. В игре    → Ctrl+C на предмет → Alt+F для цены
4. Экспорт   → .filter и .build в папки клиента PoE 2
```

**POESESSID** нужен для Trade API и live-цен uniques. Cookie хранится **только локально** и уходит лишь на `trade.pathofexile.com`.

---

## Легитимность (важно)

Exile Nexus создан как **легитимный** инструмент — в духе правил Grinding Gear Games:

| ✅ Разрешено | ❌ Нет в приложении |
|-------------|---------------------|
| Trade API, poe.ninja | Инжект в клиент PoE |
| Буфер обмена (Ctrl+C) | Чтение памяти процесса игры |
| Client.txt, экспорт `.filter` | Автоподбор, автоклик, боты |
| Overlay поверх окна | Автоматизация геймплея |

*This product isn't affiliated with or endorsed by Grinding Gear Games in any way.*

---

## Языки

Интерфейс: **English** и **Русский** (Settings → Language).

---

## Обратная связь

Баги и предложения — через Issues в репозитории разработчика или контакт автора (**SL-Studio**).

---

## Лицензия

MIT · Windows x64 · Path of Exile 2 only
