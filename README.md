# Vibe Download Site

Сайт скачивания Vibe.

## Файлы приложений

В GitHub в папке `downloads/` должны лежать ровно:

- `Vibe-Setup.exe`
- `Vibe.apk`

Имена важны: кнопки сайта ссылаются именно на них.

## Важное исправление кнопок

Кнопки Windows и Android теперь используют прямые ссылки на файлы. Предыдущая версия сначала делала `HEAD`-запрос, и на некоторых статических хостингах это могло ошибочно показывать сообщение «файл не загружен», даже когда файл существовал.

Теперь после публикации ссылки сразу открывают скачивание.

## GitHub

Структура:

```text
vibe-download/
├── index.html
├── style.css
├── assets/
│   ├── vibe-logo.png
│   ├── vibe-desktop.png
│   └── vibe-mobile.png
└── downloads/
    ├── Vibe-Setup.exe
    └── Vibe.apk
```

Обрати внимание: GitHub через браузер не принимает большие файлы как обычную загрузку. Windows-установщик размером около 93 МБ нужно загружать через Git/ GitHub Desktop (или Git LFS), а не через стандартное окно Upload files.

## Render Static Site

- Branch: `main`
- Root Directory: пусто
- Build Command: пусто
- Publish Directory: `.`
