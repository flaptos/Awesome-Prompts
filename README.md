# 🎯 Awesome-Prompts

Зеркало датасета [FamilyLinks/prompts-export-dataset](https://huggingface.co/datasets/FamilyLinks/prompts-export-dataset)

## 📊 Информация

- **Источник**: Hugging Face - FamilyLinks/prompts-export-dataset
- **Всего промптов**: 1,347,933
- **Колонки**: id, category_id, question, prompt, tags, created_at, estimated_benefits, required, difficulty_level, topic_area, subtopic, source_url, human_reviewed, reviewer_notes, title, description, reviewer_name, reviewer_title, review_text, updated_at
- **Последняя синхронизация**: 2026-05-05

## 📁 Форматы данных

- `prompts.csv` — CSV формат (основной)
- `prompts.jsonl` — JSON Lines (по одному промпту на строку)

## 🚀 Использование

```python
import pandas as pd

# Скачать с GitHub
df = pd.read_csv("https://raw.githubusercontent.com/flaptos/Awesome-Prompts/main/prompts.csv")
print(f"Всего промптов: {len(df)}")
print(df.head())
```

```javascript
// Fetch as JSONL
const response = await fetch('https://raw.githubusercontent.com/flaptos/Awesome-Prompts/main/prompts.jsonl');
const text = await response.text();
const prompts = text.split('\n').map(line => JSON.parse(line));
```

## 📈 Структура

| Колонка | Описание |
|---------|----------|
| `id` | Уникальный идентификатор промпта |
| `question` | Вопрос/запрос |
| `prompt` | Предложенный промпт |
| `tags` | Теги (JSON) |
| `difficulty_level` | Уровень сложности |
| `category_id` | ID категории |

## 🔍 Фильтрация

```python
# Примеры фильтрации
df[df['difficulty_level'] == 'beginner']  # Начальный уровень
df[df['required'] == True]  # Обязательные промпты
df[df['topic_area'] == 'AI']  # По теме
```

## 🔄 Синхронизация

Датасет обновляется автоматически при изменении исходного репозитория.

## 📝 Лицензия

Датасет принадлежит [FamilyLinks](https://huggingface.co/FamilyLinks) на [HuggingFace](https://huggingface.co/datasets/FamilyLinks/prompts-export-dataset)
