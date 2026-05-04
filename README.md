# Сайт зоопсихолога Дианы Неговоры

Репозиторий на GitHub: [github.com/pavelrysych/negovora](https://github.com/pavelrysych/negovora)

Статическая страница по материалам [Taplink — dinnega_zoopsy](https://taplink.cc/dinnega_zoopsy). Визуальный макет основан на `Desktop.pdf` (тёмная тема, иллюстрация и типографика блоков цен экспортированы из PDF).

## Содержание

- Герой: арт из PDF (`assets/hero-from-pdf.png`)
- Блок знакомства + синяя кнопка Telegram
- Тарифы: выделенный **online** с фото из PDF (`assets/pricing-feature-photo.png`), три карточки с оранжевой обводкой
- **Частые вопросы** (`#faq`): тексты с [Taplink /p/ea52bf/](https://taplink.cc/dinnega_zoopsy/p/ea52bf/)

## Запуск локально

Откройте `index.html` в браузере или поднимите простой сервер:

```bash
python3 -m http.server 8080
```

Затем откройте `http://localhost:8080`.

## Стек

HTML, CSS (без сборки). Шрифты: Google Fonts (**Cormorant Infant**, **Manrope**).

## Версионирование

В каталоге инициализирован Git — можно коммитить изменения и откатываться к прежним версиям.
