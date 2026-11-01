# Лабораторная работа 4 - Online Shoppers Purchasing Intention

## Описание

Практическая работа по машинному обучению на датасете **Online Shoppers Purchasing Intention Dataset**.

Цель работы - пройти полный цикл ML-проекта: от анализа данных и Feature Engineering до обучения ансамблевых моделей, оценки качества и интерпретации результатов с помощью SHAP.

## Что выполнено

1. Проведён исследовательский анализ данных (EDA) и построены визуализации.
2. Проверены пропущенные значения, нули и дубликаты.
3. Выполнена предобработка данных.
4. Созданы дополнительные признаки с помощью **Feature Engineering**.
5. Обработаны категориальные признаки.
6. Данные разделены на обучающую и тестовую выборки.
7. Обучены модели **Random Forest, XGBoost, LightGBM и CatBoost**.
8. Выполнено сравнение качества моделей.
9. Проведена настройка гиперпараметров с помощью **Optuna**.
10. Построены матрицы ошибок и ROC-кривые.
11. Проанализирована важность признаков.
12. Выполнена интерпретация предсказаний с помощью **SHAP**.

## Результаты

Качество моделей оценивается с помощью метрик классификации:

1. Accuracy - доля правильных предсказаний.
2. Precision - точность положительных предсказаний.
3. Recall - полнота обнаружения покупок.
4. F1-score - гармоническое среднее Precision и Recall.
5. ROC-AUC - способность модели различать классы.

Результаты моделей представлены в сравнительной таблице в ноутбуке.

## Датасет

**Online Shoppers Purchasing Intention Dataset**  
Источник: UCI Machine Learning Repository  
https://archive.ics.uci.edu/dataset/468/online+shoppers+purchasing+intention+dataset

Датасет содержит 12 330 наблюдений и 18 исходных признаков. Целевая переменная **Revenue** показывает, совершил ли пользователь покупку.

## Структура проекта

```text
lab-4-online-shoppers/
├── README.md
├── features_info.md
├── notebook.ipynb
├── requirements.txt
├── data/
├── models/
└── examples/
```

### Основные файлы

1. **notebook.ipynb** - анализ данных, создание признаков, обучение и оценка моделей.
2. **dataset_info.md** - описание датасета и признаков.
3. **data/** - исходный датасет.
4. **models/** - сохранённые обученные модели.
5. **examples/** - графики и результаты анализа.
6. **requirements.txt** - список необходимых библиотек.

## Используемые технологии
```text
pandas>=2.0
numpy>=1.24
scikit-learn>=1.3
xgboost>=2.0
lightgbm>=4.0
catboost>=1.2
optuna>=3.5
shap>=0.44
matplotlib>=3.7
seaborn>=0.12
joblib>=1.3
requests>=2.31
jupyter>=1.0
```
## Запуск

Клонировать репозиторий:

```bash
git clone https://github.com/ZhdanovaAnna/ml-course-zhdanova.git
cd module-4-features
```

Установить зависимости:

```bash
pip install -r requirements.txt
```

Поместить датасет в папку `data/` под именем:

```text
online_shoppers_intention.csv
```

Открыть **notebook.ipynb** в Jupyter Notebook и последовательно выполнить ячейки.
