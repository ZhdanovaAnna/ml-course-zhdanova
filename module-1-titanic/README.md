# Модуль 1 - Titanic

## Описание

Практическая работа по машинному обучению на датасете **Titanic - Machine Learning from Disaster**.

Цель работы - пройти полный цикл ML-проекта: от анализа и подготовки данных до обучения моделей, оценки качества и выполнения предсказаний.

## Что выполнено

1) проведён EDA и построены визуализации
2) обработаны пропущенные значения
3) выполнен Feature Engineering
4) закодированы категориальные признаки
5) обучены модели **Logistic Regression** и **Decision Tree**
6) рассчитаны Accuracy, Precision, Recall, F1 и ROC-AUC
7) построены Confusion Matrix и ROC-кривые
8) выполнена интерпретация коэффициентов Logistic Regression и важности признаков Decision Tree
9) реализована функция `predict_passenger()`
10) выполнено 5 демонстрационных предсказаний
11) модели сохранены в `.pkl`
12) метрики и параметры сохранены в `.json`
13) реализована загрузка модели из GitHub через raw-ссылку.

## Результаты

| **Модель**          | **Accuracy** | **F1** | **ROC-AUC** |
| ------------------- | -----------: | -----: | ----------: |
| Logistic Regression |        0.804 |  0.729 |       0.849 |
| Decision Tree       |        0.782 |  0.702 |       0.813 |

**Дата обучения моделей:** 26.09.2026

## Датасет

Titanic — Machine Learning from Disaster  
Источник: Kaggle  
https://www.kaggle.com/c/titanic  

## Структура

'''
module-1-titanic/
|- README.md
|- notebook.ipynb
|- requirements.txt
|- data/
|- models/
|- examples/
'''

### Основные файлы

1) 'notebook.ipynb' - полный отчёт по Модулю 1
2) 'data/' - исходные данные
3) 'models/' - обученные модели и метаданные
4) 'examples/' - сохранённые графики
5) 'requirements.txt' - зависимости проекта.

## Запуск

Установить зависимости:

'''
pip install -r requirements.txt
'''

После этого открыть `notebook.ipynb` и выполнить ячейки последовательно.

