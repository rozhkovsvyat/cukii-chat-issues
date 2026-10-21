# Лендинг установки Cukii Chat

Статическая страница установки Cukii Chat. Публикуется на GitHub Pages workflow-ом `.github/workflows/pages.yml` при каждом изменении `site/` в `main`.

## Быстрый старт

Из корня репозитория:

```bash
cd site
python -m http.server 8080
```

Откройте в браузере: [http://127.0.0.1:8080/](http://127.0.0.1:8080/)

На Windows без Python можно использовать Node.js:

```bash
cd site
npx --yes serve -l 8080
```

## Состав

| Файл | Назначение |
|------|------------|
| `index.html` | Страница установки (английский текст) |
| `styles.css` | Стили без сборки и внешних CDN |
| `assets/icon.png` | Копия `media/icon.png` без изменений |

## Что не трогать

Корневой `README.md` и шаблоны issues живут отдельно от этой страницы. Сборки нет: публикуется содержимое `site/` как есть.
