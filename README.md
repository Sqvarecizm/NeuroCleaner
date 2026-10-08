# NeuroCleaner

**Beta 1.0**

A minimalist text cleaner that rewrites your text through a chain of languages, stripping away clichés, patterns, and stylistic artifacts. Black and white. Nothing extra.

---

## 🇬🇧 English

### What it does

NeuroCleaner takes your Russian text and runs it through a chain of translations:

**Russian → Spanish → Arabic → English → Russian**

Each step restructures the sentence, breaks word order, and replaces direct meanings with equivalents. When the text comes back to Russian, it reads as a "cleaned" version — same meaning, different phrasing.

This is a classic technique for paraphrasing and de-templating text. Useful when you need to:
- Break up repetitive or formulaic writing
- Get a fresh angle on a draft
- Strip out stylistic clichés

### How to use

1. Paste your Russian text into the left panel
2. Wait for the automatic translation, or click **Обработать** (Process)
3. Copy the result from the right panel with the **Копировать** (Copy) button

### Running locally

The site uses the Google Translate API, which browsers block from `file://` origins. You need a local server.

**Requirements:** Python 3 (already on macOS and most Linux systems)

```bash
cd /path/to/NeuroCleaner
python3 -m http.server 8000
```

Then open:

```
http://localhost:8000/NeuroClean.html
```

To stop the server, press `Ctrl+C` in the terminal.

### Tech stack

- Pure HTML, CSS, JavaScript — no frameworks, no build step
- Single file (`NeuroClean.html`)
- Google Translate public API for translation
- Press Start 2P font for the version badge

### Design

Minimalism. White background, black text, thin 1px borders. No shadows, no rounded corners, no gradients. The interface is two panels side by side (stacked on mobile) with a progress indicator.

### Known limitations

- Depends on Google Translate API, which may be blocked in some regions or require a VPN
- Free API endpoint has informal rate limits
- Currently only handles Russian as the source language

### Roadmap

- [ ] Configurable language chain
- [ ] Dark theme
- [ ] Diff highlighting between input and output
- [ ] Multiple cleaning presets (soft / hard / extreme)
- [ ] Character and word counter
- [ ] Save result as .txt

---

## 🇷🇺 Русский

### Что это

NeuroCleaner берёт ваш русский текст и прогоняет его через цепочку переводов:

**Русский → Испанский → Арабский → Английский → Русский**

На каждом шаге структура предложения перестраивается, порядок слов ломается, прямые значения заменяются эквивалентами. Когда текст возвращается в русский, он читается как «очищенная» версия — тот же смысл, другая формулировка.

Это классический приём для перефразирования и «очистки» текста от шаблонов. Полезно, когда нужно:
- Разбить повторы и шаблонные конструкции
- Взглянуть на черновик под другим углом
- Убрать стилистические клише

### Как пользоваться

1. Вставьте русский текст в левое окно
2. Дождитесь автоматического перевода или нажмите **Обработать**
3. Скопируйте результат из правого окна кнопкой **Копировать**

### Запуск локально

Сайт использует Google Translate API, а браузеры блокируют запросы к нему из `file://`. Нужен локальный сервер.

**Что нужно:** Python 3 (уже есть на macOS и большинстве Linux)

```bash
cd /путь/к/NeuroCleaner
python3 -m http.server 8000
```

Затем откройте:

```
http://localhost:8000/NeuroClean.html
```

Чтобы остановить сервер — `Ctrl+C` в терминале.

### Технологии

- Чистые HTML, CSS, JavaScript — без фреймворков и сборки
- Один файл (`NeuroClean.html`)
- Публичный API Google Translate для перевода
- Шрифт Press Start 2P для бейджа версии

### Дизайн

Минимализм. Белый фон, чёрный текст, тонкие границы 1px. Без теней, скруглений и градиентов. Интерфейс — две панели рядом (на мобильных — друг под другом) с индикатором прогресса.

### Известные ограничения

- Зависит от Google Translate API, который может быть заблокирован в некоторых регионах или требовать VPN
- У бесплатного API есть неформальные лимиты по частоте запросов
- Пока поддерживает только русский как исходный язык
- Также есть проблема с некоторыми нейросетями, проверка была сделана на ChatGPT, Gemini, DeepSeek, Из них очистку смог пройти только ChatGPT, незнаю что может быть связано с этим, но как только найду причину фиксну.

### Планы

- [ ] Настраиваемая цепочка языков
- [ ] Тёмная тема
- [ ] Подсветка различий между исходным и готовым текстом
- [ ] Несколько пресетов очистки (мягкая / жёсткая / экстремальная)
- [ ] Счётчик символов и слов
- [ ] Сохранение результата в .txt

---

## License

MIT

## Author

Created by **Sqvarecizm, LaQu**
