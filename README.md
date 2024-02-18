# SmokingTrouble

**Задача**: Это задача классификации на предсказание курильщиков по клиническим показаниям на основе файла с тренировочными данными. Файл представляет собой набор биометрических и клинических показателей людей и значения целевого признака (курильщик человек или нет). Предсказание модели будет оцениваться по F-мере (F1). F-мера представляет собой гармоническое среднее между точностью и полнотой, веса которых заданы одинаковые  

**Стек**: python, библиотеки pandas, catboost, sklearn, phik, matplotlib.  

**Процесс**: Загрузил файл с контрольными данными в датафрейм. Провёл EDA. Проанализировал влияние на целевой признак по Фику и на основе корреляционной матрицы. Использовал модель Catboost: разбил выборку на тренировочную и валидационную, настроил параметры модели, подобрал оптимальный набор признаков, включаемых в модель. Провёл обучение модели на тренировочной выборке с проверкой на валидационной, затем - на всех доступных данных. Далее загрузил в датафрейм файл с тестовыми данными. Провёл предсказание целевого признака и полученные данные выгрузил в csv-файл для дальнейшей оценки на платформе Kaggle.  

**Результат**: Модель показала неплохой результат, с значением F1 0.4491. В частности, в октябре 2023г позиция в рейтинге была 5 из 39, в настоящее время (февраль 2024) - 8 из 55 (модель за этот период не улучшалась). [Ссылка на соревнование на Kaggle](https://www.kaggle.com/competitions/leopard-challenge-classification/overview)

Classification task for Leopard Challenge
This is a classification task to predict smokers based on clinical indicators. The model's prediction will be evaluated using the F-measure (F1). The weights for precision and recall are equal. Using pandas, catboost, and phik, a dataset investigation was conducted, an optimal set of parameters and variables was selected, and classification was performed on a test dataset to identify smokers. The position in the ranking is 5/39 (October 2023).

https://www.kaggle.com/competitions/leopard-challenge-classification/overview
