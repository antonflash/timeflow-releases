# TIMEFLOW

Таймер робочих проєктів для Windows 11: один активний таймер, підсумок за день, звіти й передача часу в ClickUp.

![TIMEFLOW під час роботи](screenshots/running.png)

### ⬇️ [Завантажити останню версію](https://github.com/antonflash/timeflow-releases/releases/latest)

Потрібен файл `TIMEFLOW-Setup-X.Y.Z.exe` у розділі **Assets**.

> Код TIMEFLOW закритий. Тут лежать лише готові інсталятори, з яких програма сама оновлюється.

## Встановлення

1. Завантаж `TIMEFLOW-Setup-X.Y.Z.exe` і запусти його. Права адміністратора не потрібні: програма ставиться у твій профіль, ярлики з'являються в меню «Пуск» і на робочому столі.
2. Інсталятор не має цифрового підпису, тож Windows SmartScreen може показати синє вікно «Windows захистила ваш ПК». Натисни **Докладніше** → **Виконати в будь-якому разі**.

## Оновлення

Нові версії TIMEFLOW завантажує сам, у фоні. Коли оновлення готове, зліва внизу в панелі проєктів з'являється салатовий значок «Оновити до…». Клік перезапускає програму вже з новою версією. Якщо не клікати, оновлення встановиться, коли закриєш програму.

![Значок оновлення](screenshots/update.png)

## Як це виглядає

| Таймер іде | Пауза |
|---|---|
| ![Таймер іде](screenshots/running.png) | ![Пауза](screenshots/paused.png) |

Кільце навколо Play/Pause біжить у такт із секундами:

![Анімація кільця](screenshots/ring.gif)

| Вузьке вікно | Передача часу в ClickUp |
|---|---|
| ![Вузьке вікно з рейкою проєктів](screenshots/compact.png) | ![Передача в ClickUp](screenshots/transfer.png) |

| Новий проєкт | Звіти |
|---|---|
| ![Новий проєкт](screenshots/project.png) | ![Звіти](screenshots/reports.png) |

Скріншоти зроблено з тестовими проєктами. На Windows вікно ще й зі «склом» (розмиття фону) і шрифтом Bahnschrift.

## Можливості

- Один активний таймер: Play на іншому проєкті сам ставить попередній на паузу.
- «Сьогодні загалом» і звіти за день, тиждень, місяць і весь час, експорт у CSV.
- Передача часу в задачу ClickUp за посиланням, ID або назвою.
- Закріплені проєкти, кольори, пошук; вузьке вікно з компактною рейкою проєктів.
- Значок у треї й міні-режим поверх інших вікон.
- «Ти ще працюєш?»: після години без клавіатури й миші TIMEFLOW питає, чи рахувати цей час.
- Щоденна автокопія даних у `Документи\TIMEFLOW\backups`.

## Дані та приватність

- Усе зберігається тільки на твоєму комп'ютері. TIMEFLOW нікуди не надсилає дані, крім ClickUp, і то лише коли ти сам передаєш час.
- Токен ClickUp зберігається зашифрованим засобами Windows.
- Програма звертається до цього репозиторію тільки щоб перевірити оновлення.

## Як видалити

**Параметри Windows** → **Програми** → **Встановлені програми** → TIMEFLOW → **Видалити**.
Дані (проєкти, звіти, налаштування) лишаються в `%APPDATA%\timeflow-prototype`, тож після повторного встановлення все буде на місці. Щоб прибрати їх повністю, видали цю папку вручну.

---

## English

**TIMEFLOW** is a project timer for Windows 11: one running timer, a daily total, reports and sending time to ClickUp.

### ⬇️ [Download the latest version](https://github.com/antonflash/timeflow-releases/releases/latest)

Get `TIMEFLOW-Setup-X.Y.Z.exe` under **Assets**.

> The TIMEFLOW source code is closed. This repository only holds the installers the app updates itself from.

**Install.** Run `TIMEFLOW-Setup-X.Y.Z.exe`. No administrator rights are needed: it installs into your user profile and adds Start menu and desktop shortcuts. The installer is not code-signed, so Windows SmartScreen may show "Windows protected your PC": click **More info** → **Run anyway**.

**Updates.** TIMEFLOW downloads new versions by itself in the background. When one is ready, a lime-green "Update to…" icon appears at the bottom left of the project list; a click restarts the app on the new version. Otherwise it installs when you close the app.

**Features.**
- One running timer: pressing Play on another project pauses the previous one.
- "Today in total" and reports for the day, week, month and all time, CSV export.
- Send time to a ClickUp task by link, ID or name.
- Pinned projects, colours, search; a narrow window with a compact project rail.
- Tray icon and an always-on-top mini mode.
- "Still working?": after an hour without keyboard or mouse, TIMEFLOW asks whether that time counts.
- Daily automatic backup in `Documents\TIMEFLOW\backups`.

**Data and privacy.** Everything stays on your computer. Nothing is sent anywhere except to ClickUp, and only when you send time yourself. The ClickUp token is stored encrypted by Windows. The app contacts this repository only to check for updates.

**Uninstall.** **Windows Settings** → **Apps** → **Installed apps** → TIMEFLOW → **Uninstall**. Your data stays in `%APPDATA%\timeflow-prototype`, so a reinstall picks it up again; delete that folder to remove it completely.

The screenshots above use test projects. On Windows the window also has the glass (blurred background) look and the Bahnschrift font.
