# Workout App — трекер тренировок Тимура

Одностраничное PWA-приложение (один файл `index.html`), открывается на iPhone как веб-приложение.

## Ссылки

- **Приложение:** https://mtimuru-bit.github.io/workout-app/
- **Репозиторий:** https://github.com/mtimuru-bit/workout-app (public)
- **Локальная папка:** `C:\Users\Lenovo\Диалоги с Claude\workout-app\`
- Старая версия: `benevolent-cocada-5e35f8.netlify.app` (Netlify, работает параллельно; история в её localStorage не переносится автоматически)

## Как устроен деплой

- Хостинг — GitHub Pages (legacy build) с ветки `main`, корень `/`.
- Любой `git push` в `main` → Pages пересобирает сайт за ~30–60 секунд.
- Netlify и токены GitHub НЕ используются: обновления идут через Claude Code на этом ПК (git настроен, GitHub CLI авторизован как `mtimuru-bit`).

## Как обновить приложение

1. Править `index.html` в этой папке.
2. `git add index.html && git commit && git push`.
3. Через минуту изменения на проде; iPhone покажет баннер обновления (интервал проверки — до ~5 минут).

## Данные

Вся история тренировок хранится в localStorage на устройстве пользователя — в репозитории персональных данных нет, поэтому репо может быть публичным.

## История

- **2026-10-09** — первый деплой на GitHub Pages. Источник: `Downloads\workout_13.html` от 03.05.2026 (новейшая из 14 версий workout*.html в Downloads). Создан репозиторий, включён Pages, проверен HTTP 200.
