# Roadmap

## Сделано

- [x] Разбор слоёв из JSON опубликованного `figma.site` и вёрстка под фрейм **Desktop**: порядок секций как в экспорте, не под старую статическую версию сайта.
- [x] Герой: отступ блока текста под картинку; IG по середине «Диана»; топ первого абзаца формулой под топ IG; итого низ колонок + Telegram как раньше.
- [x] Блок online: порядок «Самое популярное → заголовок → цены → описание → список → coral bar», параллельно фото; три тариф-карты с оранжевой обводкой и нижним bar.
- [x] Нижний блок FAQ: содержание из Taplink `/p/ea52bf/` (JSON `window.data`), раскладка аккордеоном через `<details>`.
- [x] SEO: усилены title/description/robots, canonical + hreflang, Open Graph и Twitter Card, preload героя; JSON-LD (`WebSite`, `Person`, `ProfessionalService`); `robots.txt` и `sitemap.xml` с базовым URL `https://negovora.vercel.app` (замена при своём домене).

## Дальше

- [ ] Подстройка интерполируемых интервалов после скрин-регресса против живого viewport Figma Sites.
- [ ] GitHub Pages / домен при готовности.
