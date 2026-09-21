# Reorder Model — тестовое задание Supply Chain Data Analyst (Генерация)

Модель рекомендуемого количества к заказу по 200 SKU на дату расчёта 19.09.2025, с бэктестом на исторических данных и сравнением с базовым вариантом.

Методика, результаты и допущения — в разработке, будут описаны здесь по мере готовности решения.

## Что где лежит

```
reorder-model/
  data/                     исходные данные (candidate_data.xlsx, data_dictionary.xlsx)
  notebooks/
    reorder_model.ipynb     основной артефакт: данные → EDA → baseline → бэктест → финальный расчёт
  output/
    RecommendedOrder.xlsx   финальная таблица SKU -> RecommendedOrder
  README.md                 этот файл
  requirements.txt          зависимости для запуска ноутбука
```

## Как запустить

```
python -m venv .venv
.venv\Scripts\activate          # Windows
pip install -r requirements.txt
jupyter notebook notebooks/reorder_model.ipynb
```

Либо пересчитать без интерфейса Jupyter:

```
jupyter nbconvert --to notebook --execute --inplace notebooks/reorder_model.ipynb
```
