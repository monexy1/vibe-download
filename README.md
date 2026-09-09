# Vibe Download Site

Официальный сайт скачивания Vibe.

## Структура

- `index.html` — главная страница.
- `style.css` — оформление и адаптив.
- `assets/vibe-logo.png` — логотип Vibe.
- `assets/vibe-desktop.png` — реальный скриншот интерфейса Vibe на ПК.
- `assets/vibe-mobile.png` — реальный скриншот интерфейса Vibe на телефоне.
- `downloads/Vibe-Setup.exe` — сюда положить Windows-установщик.
- `downloads/Vibe.apk` — сюда положить Android APK.

## Как сделать кнопки скачивания рабочими

1. Собери Windows установщик и назови его **Vibe-Setup.exe**.
2. Собери Android APK и назови его **Vibe.apk**.
3. Положи оба файла в папку `downloads/` в этом GitHub-репозитории.
4. Сделай Commit changes.
5. Render автоматически обновит Static Site.
6. Кнопки «Скачать для Windows» и «Скачать APK Android» начнут отдавать реальные файлы.

Пока файлов нет, нажатие на кнопку показывает понятное окно вместо пустой/404-страницы.

## GitHub Pages / Render

`index.html` находится в корне репозитория. Для Render Static Site:
- Branch: `main`
- Root Directory: пусто
- Build Command: пусто
- Publish Directory: `.`

После добавления APK и EXE ничего в HTML менять не нужно.
