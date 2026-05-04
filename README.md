# Сайт Дианы Неговоры (вёрстка под опубликованный Figma-макет)

Статический лендинг: `index.html` + `styles.css`. Интерполяции по **слоям Desktop** из JSON `figma.site` (шрифты и порядок блоков совпадают с опубликованной страницей).

Секция **«Частые вопросы»**: тексты блоков свёртывания взяты с
[этой страницы Taplink](https://taplink.cc/dinnega_zoopsy/p/ea52bf/) (`window.data`), механика — стандартные `<details>/<summary>`
(без JavaScript).

**Ссылки на контакты**

- Telegram: `https://t.me/dinnega` — главная кнопка и все «Записаться».
- Instagram: `https://www.instagram.com/dinnega_zoopsy/` — иконка в шапке.
- Надпись «Частые вопросы» в шапке ведёт к нижнему блоку `#faq-content`.

Изображения в `assets/` скачаны с CDN того же сайта (`_assets/v11/*.png`). Локально:

```bash
python3 -m http.server 8080
```

Герой («intro»): на десктопе верх первого абзаца справа и **верх иконки Instagram** на одном уровне; низ строки «Зоопсихолог, Тбилиси» = низ ссылки «Частые вопросы», кнопка Telegram вертикально по центру зазора между абзацами и FAQ.

Шрифты: **Cormorant Infant**, **Inter** (Google Fonts). В шапке: имя **Cormorant Infant Regular 96 px**; строка «Зоопсихолог, Тбилиси» — **Cormorant Infant Regular 24 px** (как в Figma; на узких экранах подзаголовок слегка уменьшен через `clamp`). Абзацы в правой колонке героя — **Inter Light (300) / 14 px**, line-height auto, без трекинга — как в Figma.
