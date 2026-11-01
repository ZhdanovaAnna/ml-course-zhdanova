# Описание датасета Online Shoppers Purchasing Intention

## 1. Датасет и источник

В проекте используется датасет **Online Shoppers Purchasing Intention Dataset** из репозитория UCI Machine Learning Repository:

https://archive.ics.uci.edu/dataset/468/online+shoppers+purchasing+intention+dataset

## 2. Данные

Датасет содержит 12 330 наблюдений и 18 исходных признаков, включая целевую переменную `Revenue`. Каждая строка соответствует одному сеансу посещения интернет-магазина.

Целевая переменная **`Revenue`**:
1. `True` - покупка совершена.
2. `False` - покупка не совершена.

## 3. Основные признаки

Признаки описывают:

1. Посещение страниц: `Administrative`, `Informational`, `ProductRelated`.
2. Время просмотра страниц: `Administrative_Duration`, `Informational_Duration`, `ProductRelated_Duration`.
3. Поведение пользователей: `BounceRates`, `ExitRates`, `PageValues`, `SpecialDay`.
4. Характеристики посещения: `Month`, `Weekend`, `VisitorType`.
5. Технические и географические данные: `OperatingSystems`, `Browser`, `Region`, `TrafficType`.

## 4. Инженерия признаков

В работе создаются дополнительные признаки, характеризующие активность пользователей, количество посещённых страниц, время просмотра и особенности поведения. Целевая переменная `Revenue` не используется как входной признак модели.

## 5. Модели и оценка

Используются четыре ансамблевые модели: **Random Forest, XGBoost, LightGBM и CatBoost**.

Качество оценивается с помощью Accuracy, Precision, Recall, F1-score и ROC-AUC. Для интерпретации предсказаний применяется SHAP.

## 6. Цель использования

Датасет используется для прогнозирования вероятности покупки, выявления значимых факторов поведения посетителей и сравнения моделей машинного обучения.