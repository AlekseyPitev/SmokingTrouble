# SmokingTrouble

Задача: Это задача классификации на предсказание курильщиков по клиническим показаниям. На основе файла с тренировочными данными, представляющими собой набор различных биометрических и клинических показателей людей и значение целевого признака (является ли человек курильщиком или нет). Предсказание модели будет оцениваться по F-мере (F1). F-мера представляет собой гармоническое среднее между точностью и полнотой. Веса для точности и полноты заданы одинаковые.  
Стек: python, библиотеки pandas, catboost, sklearn, phik.  
Процесс: Загружается файл с контрольными данными в датафрейм. Проводится EDA. Анализируется влияние на целевой признак по Фику и на основе корреляционной матрицы. Использую модель Catboost. Выборка разбивается на тренировочную и валидационную, настраиваются параметры модели. Подбирается оптимальный набор признаков, включаемых в модель. Проводится обучение модели на тренировочной модели с проверкой на валидационной, затем на всех доступных данных. Затем загружается в датафрейм файл с тестовыми данными. Проводится предсказания целевого признака и полученные данные выгружаются в csv-файл для дальнейшей оценки на платформе Kaggle.  
Результат: Модель показала неплохой результат, с значением F1 0.4491. В частности, в октябре 2023г позиция в рейтинге была 5 из 39, в настоящее время (февраль 2024) - 8 из 55 (модель за этот период не улучшалась). [Ссылка на соревнование на Kaggle](https://www.kaggle.com/competitions/leopard-challenge-classification/overview)

Classification task for Leopard Challenge
This is a classification task to predict smokers based on clinical indicators. The model's prediction will be evaluated using the F-measure (F1). The weights for precision and recall are equal. Using pandas, catboost, and phik, a dataset investigation was conducted, an optimal set of parameters and variables was selected, and classification was performed on a test dataset to identify smokers. The position in the ranking is 5/39 (October 2023).

https://www.kaggle.com/competitions/leopard-challenge-classification/overview
