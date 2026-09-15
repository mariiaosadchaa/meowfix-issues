name: Bug Report
description: Повідомити про помилку у проекті
title: "[BUG]: "
labels: ["bug"]
body:
  - type: markdown
    attributes:
      value: |
        Дякуємо за знайдену помилку! Будь ласка, заповніть форму нижче.

  - type: textarea
    id: description
    attributes:
      label: Опис проблеми
      description: Коротко опишіть, що працює неналежним чином.
      placeholder: При кліку на кнопку...
    validations:
      required: true

  - type: textarea
    id: steps
    attributes:
      label: Кроки для відтворення
      description: Опишіть покроково, як відтворити помилку.
      placeholder: |
        1. Перейти на сторінку...
        2. Натиснути...
        3. Отримати помилку...
    validations:
      required: true

  - type: textarea
    id: expected
    attributes:
      label: Очікувана поведінка
      description: Опишіть, що мало відбутися.
    validations:
      required: true

  - type: input
    id: environment
    attributes:
      label: Середовище / ОС / Браузер
      placeholder: macOS / Chrome 120 / v1.2.0
    validations:
      required: false

  - type: textarea
    id: additional
    attributes:
      label: Додаткова інформація чи скріншоти
      description: Сюди можна перетягнути скріншоти або вставити логи.
    validations:
      required: false
