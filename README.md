# Why not Goddess?

Статический сайт проекта Why not Goddess, опубликованный в Cloudflare Pages.

## Структура

- `public/` — готовые файлы сайта;
- `.github/workflows/deploy.yml` — автоматическая публикация в Cloudflare Pages после изменений в ветке `main`.

## Автоматическая публикация

В настройках GitHub-репозитория нужны два секрета Actions:

- `CLOUDFLARE_ACCOUNT_ID` — ID аккаунта Cloudflare;
- `CLOUDFLARE_API_TOKEN` — токен с правом `Account / Cloudflare Pages / Edit`.

После каждого push в `main` workflow публикует каталог `public/` в существующий проект Cloudflare Pages `whynotgoddess`.

