# Прогноз вероятности совершения заказа клиентами в период с 01.11.11 по 30.11.11

## Описание проекта

Для анализа данных и построения модели предоставлен датасет, cодержащий информацию о совершении заказов клиентами в период с 01.11.11 по 30.11.11
<br>Проект завершен.

## Цель проекта
- Для каждого клиента, который делал заказ в период с 01.12.10 по 31.10.11, необходимо спрогнозировать вероятность совершения заказа в период с 01.11.11 по 30.11.11;
- Обосновать выбор модели и метрики качества;
- Дать рекомендации относительно перспектив дальнейшего исследования этого массива данных.

## Ход выполнения проекта
- Предобработка данных заключалась в удалении пропусков в датасете, очистке от выбросов и изменении типов данных. Далее датасет былтрансформирован в новый, где объектами выступают клиенты, а признаками являются факт совержения покупки в определенный месяц года¶.

- Проведенный анализ данных  позволил спрогнозировать вероятность совершения заказа для каждого клиента в период с 01.11.11 по 30.11.11;

- Обучение моделей и проверка их на кросс-валидации позволила определить лучшую для этого модель. Ей оказалась RandomForestClassifier. Подбор оптимальных параметров осуществлялся с помощью функции GridSearchCV. Средний показатель метрики F1_score на кросс-валидации равняется 0.62.

- Финальным шагом стало предсказание и запись в файл answer.csv предсказаний вероятностей  совершении заказов клиентами в период с 01.11.11 по 30.11.11. 

## Итоги проекта

- Проведена предобработка и исследование данных;
- Протестированы различные модели машинного обучения с подбором гиперпараметров и кросс-валидациецией;
- Для каждого клиента, который делал заказ в период с 01.12.10 по 31.10.11, спрогнозированы вероятности совершения заказа в период с 01.11.11 по 30.11.11;
- Обоснованы выбор модели и метрики качества;
- Даны рекомендации относительно перспектив дальнейшего исследования этого массива данных.

В проекте использованы библиотеки:
- pandas
- matplotlib
- seaborn
- sklearn
- numpy
- lightgbm
