# Датасет "Обзоры судебной практики судов Российской Федерации"

Этот репозиторий содержит датасет обзоров судебной практики высших судов Российской Федерации. **Важно отметить, что данный датасет не является исчерпывающим и представляет собой лишь выборку документов.**

Документы могут быть использованы для анализа, машинного обучения и других исследований в области права.

## Состав датасета

Датасет включает в себя следующее количество документов по каждому суду:

*   **Обзор Верховного Суда Российской Федерации:** 435 документов
*   **Обзор Высшего Арбитражного Суда Российской Федерации:** 122 документа
*   **Обзор Конституционного суда Российской Федерации:** 54 документа
*   **Обзор Суда по интеллектуальным правам Российской Федерации:** 6 документов

**Всего в датасете 617 документов.**

## Структура данных

Каждый документ представляет собой отдельный JSON-файл со следующей структурой:

```json
{
  "title": "Название документа",
  "type": "Тип документа (например, Обзор Верховного Суда Российской Федерации)",
  "text": "Полный текст документа..."
}
```

*   `title`: Официальное название обзора.
*   `type`: Категория документа, указывающая на принадлежность к определенному суду.
*   `text`: Полное текстовое содержание документа.

## Важное замечание об анонимизации данных

Для защиты персональных данных была проведена их автоматическая санитация с использованием библиотеки **spaCy** и языковой модели `ru_core_news_lg`.

**Внимание:** Автоматическая обработка не гарантирует 100% точности. Возможны ложные срабатывания:
*   Некоторые персональные данные (ФИО, адреса и т.д.) могли остаться в текстах.
*   Часть информации, не являющейся персональными данными, могла быть ошибочно удалена.

Рекомендуется проводить дополнительную проверку данных перед их использованием в публичных или коммерческих проектах.

## Лицензия

Этот датасет распространяется по лицензии [Creative Commons Zero v1.0 Universal (CC0 1.0)](https://creativecommons.org/publicdomain/zero/1.0/deed.ru).

Это означает, что вы можете свободно копировать, изменять, распространять и использовать данные, в том числе в коммерческих целях, без необходимости получения разрешения.

---

# Judicial Practice Reviews of the Courts of the Russian Federation

This repository contains a dataset of judicial practice reviews from the higher courts of the Russian Federation. **It is important to note that this dataset is not exhaustive and represents only a selection of documents.**

The documents can be used for analysis, machine learning, and other research in the legal field.

## Dataset Composition

The dataset includes the following number of documents for each court:

*   **Review of the Supreme Court of the Russian Federation:** 435 documents
*   **Review of the Supreme Arbitration Court of the Russian Federation:** 122 documents
*   **Review of the Constitutional Court of the Russian Federation:** 54 documents
*   **Review of the Intellectual Property Rights Court of the Russian Federation:** 6 documents

**Total documents in the dataset: 617.**

## Data Structure

Each document is a separate JSON file with the following structure:

```json
{
  "title": "Document title",
  "type": "Document type (e.g., Review of the Supreme Court of the Russian Federation)",
  "text": "Full text of the document..."
}
```

*   `title`: The official title of the review.
*   `type`: The document category, indicating which court it belongs to.
*   `text`: The full text content of the document.

## Important Note on Data Anonymization

To protect personal data, it has been automatically sanitized using the **spaCy** library and the `ru_core_news_lg` language model.

**Warning:** Automated processing does not guarantee 100% accuracy. False positives/negatives may occur:
*   Some personal data (full names, addresses, etc.) may remain in the texts.
*   Some information that is not personal data may have been mistakenly removed.

It is recommended to perform additional verification of the data before using it in public or commercial projects.

## License

This dataset is licensed under [Creative Commons Zero v1.0 Universal (CC0 1.0)](https://creativecommons.org/publicdomain/zero/1.0/).

This means you are free to copy, modify, distribute, and use the data, including for commercial purposes, without asking for permission.
