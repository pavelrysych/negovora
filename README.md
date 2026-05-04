# Сайт Дианы Неговоры (вёрстка под опубликованный Figma-макет)

Статический лендинг: `index.html` + `styles.css`. Интерполяции по **слоям Desktop** из JSON `figma.site` (шрифты и порядок блоков совпадают с опубликованной страницей).

**Функционал ссылок (как договорено):**

- Telegram: `https://t.me/dinnega` — главная кнопка и все «Записаться».
- Instagram: `https://www.instagram.com/dinnega_zoopsy/` — иконка в шапке.
- «Частые вопросы» над шапкой ведёт к нижнему блоку `#faq-content`.

Изображения в `assets/` скачаны с CDN того же сайта (`_assets/v11/*.png`). Локально:

```bash
python3 -m http.server 8080
```

Шрифты: **Cormorant Infant**, **Inter** (Google Fonts). Системная **Georgia** для блока имени.
