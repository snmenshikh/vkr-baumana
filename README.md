# Выпускная квалификационная работа по курсу "Инженер данных PRO" слушателя группы 12903 ЦДО МГТУ им.Баумана Меньших С.Н. 
## Тема: Классификация государственных контрактов по предмету закупки
Основной задачей выполнения ВКР является анализ современных моделей машинного обучения и исследование программных методов классификации с целью определения тех из них, что наиболее точно могут решить задачу классификации предмета контракта, написанного на естественном языке, для определения верно соответствующего ему кода ОКПД2.
В рамках выполнения ВКР проведено:
* сбор данных о закупках из CSV-файла;
* предварительная обработка и разведочный анализ исходного датасета;
* лемматизация предмета контракта с использованием русской модели библиотеки spaCy;
* создание, обучение, применение, оценка качества работы и сравнение 7 моделей мультиклассовой классификации: логистической регрессии (Logistic Regression), случайного леса (Random Forest), градиентного бустинга (Gradient Boosting), метода опорных векторов (Support Vector Machines), наивного байесовского классификатора (Naive Bayes), экстремального градиентного бустинга (XGBoost) и нейронной сети (MLP, многослойный перцептрон);
* сохранение выбранной модели и ее применение для классификации нового контракта.

Таблица показателей качества лучших моделей (на тестовой выборке):
Наименование модели       | Accuracy | F1-score
--------------------------|----------|----------
Logistic Regression       |   0,65   |   0,72
Extreme Gradient Boosting |   0,65   |   0,73
Multilayered Perceptron   |   0,__   |   0,__

В ходе выполнения ВКР получены и проанализированы результаты классификации предметов контрактов, записанных на естественном языке, для целей определения групп кодов ОКПД2, к которым принадлежит закупка. Для классификации были использованы обученные на реальных данных модели. Наилучшие результаты показаны алгоритмами **логистической регрессии, экстремального градиентного бустинга и нейронной сети**. Эти модели в совокупности с разработанным приложением могут быть использованы в качестве рекомендательного сервиса при осуществлении государственных закупок.
