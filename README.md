# ML-Cell-Phone-Plans
# ML: Тарифы связи
Задача: необходимо понять, какой тариф выгоднее предложить клиенту.

Были рассмотрены статистики всех признаков, гистограммы распределения всех признаков в разрезе тарифов, корреляции всех признаков с тарифом, построена диаграмма отношений между всеми парами признаков.
Была поставлена задача классификации. рассмотрены решения с помощью разных моделей, всем моделям предложены разные параметры и выбраны наилучшие.
Были исследованы модели дерева решений, случайного леса, логистической регрессии, K ближайших соседей, наивная байесовская модель и модель градиентного бустинга.
Все модели были исследованы двумя способами: были выбраны наилучшие параметры с помощью функции GridSearchCV и с помощью ручного перебора параметров в циклах.
Все полученные на валидации данные записаны в таблицу.
результаты работы моделей сравнены с помощью метрики accuracy_score.
Лучший результат на валидационной выборке показывают модель случайного леса (где параметры подобраны с помощью перебора в циклах) и модель градиентного бустинга (где параметры подобраны с помощью перебора в циклах).
Все полученные данные на тестовой выборке записаны в таблицу.
Результаты на тесте немного отличаются от результатов на валидации. Лучший результат дает модель градиентного бустинга (где параметры подобраны с помощью перебора в циклах) и модель случайного леса (где параметры подобраны с помощью перебора в циклах).
Качество исследованных моделей сравнено с качеством "простой" модели DummyClassifier().
Использована библиотека sklearn.