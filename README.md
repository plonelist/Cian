# Cian Moscow Real Estate Analysis

Проект по анализу объявлений о недвижимости Москвы и подготовке данных для модели оценки справедливой стоимости квартиры.

## Структура

- `clean_up.ipynb` - базовая проверка и очистка исходного датасета.
- `feature_engineering.ipynb` - извлечение площади, комнатности и расчет цены за квадратный метр.
- `market_analysis.ipynb` - рыночные метрики, анализ по комнатам, годам и метро.
- `data/` - сжатые CSV-файлы, которые используются в ноутбуках.

## Данные

Датасеты лежат в папке `data/` в формате `.csv.gz`.
Pandas читает такие файлы напрямую через `pd.read_csv(...)`, распаковывать вручную не нужно.

Используемые файлы:

- `data/Moscow_cleaned.csv.gz`
- `data/moscow_clean_base.csv.gz`
- `data/moscow_flats_clean.csv.gz`

## Как запустить

1. Склонировать репозиторий.
2. Установить зависимости:

```bash
pip install -r requirements.txt
```

3. Открыть ноутбуки в Jupyter Notebook или VS Code.
4. Запускать по порядку:

```text
clean_up.ipynb
feature_engineering.ipynb
market_analysis.ipynb
```

Если нужно только посмотреть готовый анализ, можно сразу открыть `market_analysis.ipynb`.
