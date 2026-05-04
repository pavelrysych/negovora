# Сайт Дианы Неговоры (вёрстка под опубликованный Figma-макет)

Статический лендинг: `index.html` + `site.css` (исторический путь `/styles.css` редиректит на `site.css`, чтобы сбросить CDN-кэши). Интерполяции по **слоям Desktop** из JSON `figma.site` (шрифты и порядок блоков совпадают с опубликованной страницей). **Фавикон:** фрагмент логотипа «Di» (бордовое на коралловом) — `assets/favicon.ico`, PNG и `apple-touch-icon`; исходник обрезки — `assets/favicon-source-di-logo.png`.

Секция **«Частые вопросы»**: тексты блоков свёртывания взяты с
[этой страницы Taplink](https://taplink.cc/dinnega_zoopsy/p/ea52bf/) (`window.data`), механика — стандартные `<details>/<summary>`
(без JavaScript).

**Ссылки на контакты**

- Telegram: `https://t.me/dinnega` — главная кнопка и все «Записаться».
- Instagram: `https://www.instagram.com/dinnega_zoopsy/` — иконка в шапке.
- Надпись «Частые вопросы» в шапке ведёт к нижнему блоку `#faq-content`.

**SEO** (поиск и соцсети):

- Усилены `<title>`, описание (`meta description`), canonical, hreflang для `ru-RU`, тема вкладки (`theme-color`).
- Разметка **Open Graph** и **Twitter Card** для превью ссылок; картинка превью — `assets/hero.png`.
- Структурированные данные **JSON-LD** (`WebSite`, `Person`, `ProfessionalService`) в `<head>` (проверка: Rich Results Test / Schema Validator).
- Файлы в корне: [`robots.txt`](robots.txt), [`sitemap.xml`](sitemap.xml).
- Абсолютный базовый URL сейчас **`https://negovora.vercel.app`** — при подключении своего домена замените его **во всех местах**: комментарий в `index.html`, URL в мета-тегах и JSON-LD, строка `Sitemap` в `robots.txt`, `<loc>` в `sitemap.xml`.

Под футером FAQ добавлен блок `<footer>`: ширина на всё «внутреннее полотно» шелла (как у героя), файл `assets/footer-illustration.png`, текст **Diana Negovora, 2026** поверх изображения с градиентом для читаемости.

Изображения в `assets/` скачаны с CDN того же сайта (`_assets/v11/*.png`). Дополнительно: свой футер-баннер `footer-illustration.png`. Локально:

```bash
python3 -m http.server 8080
```

Герой: отступ между **иллюстрацией сверху** и двухколоночным блоком (`intro__grid`); иконка Instagram по центру строки «Диана», **первая строка** правого текста опущена на `padding-top`, чтобы совпала с верхом иконки (формула от кегля); низ «Зоопсихолог, Тбилиси» совпадает с низом «Частые вопросы», Telegram между абзацами и FAQ по вертикали по центру.

Шрифты: **Cormorant Infant**, **Inter** (Google Fonts). В шапке: имя **Cormorant Infant Regular 96 px**; строка «Зоопсихолог, Тбилиси» — **Cormorant Infant Regular 24 px** (как в Figma; на узких экранах подзаголовок слегка уменьшен через `clamp`). Абзацы в правой колонке героя — **Inter Light (300) / 14 px**, line-height auto, без трекинга — как в Figma.
