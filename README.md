# Сайт зоопсихолога Дианы Неговоры

Статическая витрина: `index.html` + `styles.css`. Контент и порядок блоков совпадают с опубликованным макетом Figma Publish:  
[https://swept-coral-15784474.figma.site/](https://swept-coral-15784474.figma.site/)

Рабочие кнопки и ссылки: запись и контакты ведут в Telegram [`https://t.me/dinnega`](https://t.me/dinnega); «Частые вопросы» прокручивают к секции FAQ.

## Запуск локально

```bash
python3 -m http.server 8080
```

Откройте [http://localhost:8080](http://localhost:8080) или откройте `index.html` в браузере.

## Герой-постер (картинка по желанию)

По умолчанию верх блока воспроизводится типографикой на коралловом фоне. Чтобы подставить иллюстрацию из Figma, экспортируйте её в **`assets/poster.png`**, раскомментируйте тег `<img>` внутри `.hero-poster__inner` в `index.html` и при необходимости скройте `.hero-poster__fallback` в CSS.

Шрифты: **Baloo 2**, **Cormorant Garamond**, **Nunito Sans** (Google Fonts, кириллица).

## Версионирование

В репозитории инициализирован Git — можно откатываться к прежним версиям.
