# docs-automation-study

Учебный репозиторий по практической работе 3.4
«Автоматизация разработки технической документации: от хаоса к конвейеру».

## Что внутри

| Путь | Назначение |
|---|---|
| `docs/01_intro.md` | Введение, цели и схема процесса публикации |
| `docs/02_api.md` | Описание функции входа в API |
| `docs/03_report.md` | Отчёт о выполнении работы |
| `openapi/openapi.yaml` | Машиночитаемая спецификация OpenAPI 3.0 |
| `plantuml/sequence.puml` | Исходный текст схемы PlantUML |
| `index.html`, `assets/` | Статический сайт для GitHub Pages |

## Принципы

- единый источник документации (Single Source of Truth);
- версионирование каждого изменения через Git;
- текстовая разметка Markdown вместо «ручного» форматирования;
- автоматическая сборка сайта из репозитория;
- схемы и справочники API генерируются из текстовых исходников.

## Публикация

```bash
git remote add origin https://github.com/karnilov35-cmd/docs-automation-study.git
git push -u origin main
```

Затем: **Settings → Pages → Deploy from a branch → main → / (root)**.

