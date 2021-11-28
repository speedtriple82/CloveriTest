# CloveriTest
Ответ к тестовому заданию на стажировки Кловери
Задание:
Есть 4 набора данных:
1. о купленных билетах (идентификатор мероприятия; идентификатор участника; дата покупки; стоимость билета)
2. о возрасте и регионе участника программы (возраст — от 14 до 22, регион — один из 85 регионов РФ).
3. о мероприятиях в регионе посещения (тип организации; идентификатор мероприятия)
4. о факте посещения мероприятий (идентификатор мероприятия; идентификатор участника; дата посещения)
Ответьте на вопросы ниже.
1. Опишите, как бы вы использовали эти данные для предсказания, какое событие заинтересует участника?
2. Какие дополнительные данные могут повлиять на точность предсказаний?
3. Какую бы метрику использовали для оценки качества работы рекомендательной модели?


Для решения поставленной я бы выполнил следующие шаги:

1. Определился с таргетом. В данном случае надо понять пойдет участник программы на мероприятие или нет. Таким образом надо решать задачу классификации;
2. Используя язык программирования Python и библиотеку Pandas, выполнил  операции по объединению датасетов в один и с генерировал признак являющийся таргетом. (подробнее см. Приложение);
3. Добавил новые признаки из имеющихся, удалил ненужные (подробнее см. Приложение);
4. Провел анализ зависимости признаков на таргет, анализ корреляций числовых признаков;
5. Было бы не плохо обогатить данный датасет дополнительными данными, такими как: вид занятости участника(школьник, студент, безработный, работающий), пол участника, наличие романтических отношений, количество часов проводимых на работе/учебе. 
6. Разбил датасет на тренировочную и валидационную часть;
7. Построил базовую модель например лог регрессию;
8. Определил метрику например F1-score (еще варианты см. Приложение);
9. Построил другую модель/модели, посчитал метрику;
10. Пробовал убирать/добавлять признаки, изменять гиперпараметры модели смотреть на изменение метрики
11. Направил в продакшн(?) вариант, показывающий наилучший результат.
