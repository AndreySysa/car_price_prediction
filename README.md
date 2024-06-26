# Определение стоимости автомобилей по VIN.

[VIN-стоимость](https://github.com/AndreySysa/car_price_prediction/blob/master/Определение%20стоимости%20автомобиля%20по%20VIN.ipynb)[^1]

Перед нами стояла задача: 
- Разработка системы рекомендации стоимости автомобиля на основе его VIN номера.
- Данные были предоставлены в виде текстового документа vin_ford_train.txt 
***
Для выполнения поставленной задачи использовались следующие библиотеки и модули:
- matplotlib.pyplot: библиотека для создания статических графиков и визуализаций.
- seaborn: библиотека для визуализации данных с высокоуровневым интерфейсом.
- pandas: библиотека для работы с данными в виде таблиц (DataFrame).
- numpy: библиотека для работы с многомерными массивами и математическими функциями.
- optuna: библиотека для оптимизации гиперпараметров моделей машинного обучения.
- re: модуль для работы с регулярными выражениями.
- sklearn.model_selection.KFold: класс для разделения данных на фолды в кросс-валидации (KFold).
- sklearn.model_selection.train_test_split: функция для разделения данных на обучающую и тестовую выборки.
- sklearn.model_selection.cross_val_score: функция для оценки модели с использованием кросс-валидации.
- sklearn.preprocessing.StandardScaler: класс для стандартизации данных (Standardization).
- sklearn.preprocessing.OneHotEncoder: класс для преобразования категориальных переменных в числовые с помощью метода One-Hot Encoding.
- sklearn.ensemble.RandomForestRegressor: класс для обучения случайного леса (Random Forest).
- sklearn.metrics.mean_squared_error: функция для вычисления среднеквадратичной ошибки (Mean Squared Error).
- sklearn.dummy.DummyRegressor: класс для создания простой базовой модели, используемой как эталон при оценке других моделей.
- catboost.CatBoostRegressor: класс для обучения градиентного бустинга на деревьях (CatBoost).
- lightgbm.LGBMRegressor: класс для обучения градиентного бустинга на деревьях (LightGBM).
- time: модуль для работы со временем, позволяющий измерять время выполнения операций.
***
**Вывод:**
***
- Модель **LGBMRegressor(bagging_fraction=0.3, feature_fraction=0.5, learning_rate=0.2, min_child_samples=45, n_estimators=99, num_leaves=128, reg_alpha=0.5, reg_lambda=1.0, random_state=12345, n_jobs=-1)** предсказывает точнее, чем простая модель DummyRegressor() и работает быстро.
- Выбранная модель соответствует критериям, которые важны заказчику.


[^1]:Для корректного просмотра Jupyter notebook с работающим содержанием, пожалуйста, используйте следующую ссылку:
[Определение стоимости автомобилей по VIN](https://nbviewer.jupyter.org/github/AndreySysa/car_price_prediction/blob/master/Определение%20стоимости%20автомобиля%20по%20VIN.ipynb)
Просто кликните на ссылку, и nbviewer отобразит notebook с интерактивными ссылками.
