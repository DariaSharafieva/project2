# Проект 1. Работа с данными о резюме

## Оглавление  
[1. Описание проекта](#описание-проекта)  
[2. Какой кейс решаем?](#какой-кейс-решаем)  
[3. Краткая информация о данных](#краткая-информация-о-данных)  
[4. Этапы работы над проектом](#этапы-работы-над-проектом)  
[5. Результат](#результат)    
[6. Выводы](#выводы) 

### Описание проекта    
Проект состоит из 4 частей:
1. Базовый анализ структур данных
2. Преобразование данных
3. Разведывательный анализ
4. Очистка данных

[к оглавлению](#оглавление)

___
### Какой кейс решаем?    
Отрабатываем основные этапы работы с данными на примере датасета о резюме
___
### Краткая информация о данных
[Датасет Head Hanter](https://drive.google.com/file/d/1Kb78mAWYKcYlellTGhIjPI-bCcKbGuTn/view)

Датасет представляет из себя набор данных в формате csv, состоящий из 44744 строк

До преобразования данных DataFrame содержит 12 признаков:
+ Пол, возраст
+ Ищет работу на должность:
+ Город, переезд, командировки 
+ Занятость 
+ График
+ Опыт работы
+ Последнее/нынешнее место работы 
+ Последняя/нынешняя должность
+ Образование и ВУЗ
+ Обновление резюме
+ Авто

Дополнительно используется [таблица для конвертации валют](https://lms-cdn.skillfactory.ru/assets/courseware/v1/15abf80f45a2f3e93c3274101b451c67/asset-v1:SkillFactory+DSPR-2.0+14JULY2021+type@asset+block/ExchangeRates.zip)

[к оглавлению](#оглавление)

___
### Этапы работы над проектом  
1. __Производим исследование структуры дынных__
+ читаем данные с помощью библиотеки Pandas
+ выводим несколько первых (последних) строк таблицы, чтобы убедиться в том, что данные не повреждены. Ознакомливаемся с признаками и их структурой
+ выводим основную информацию о числе непустых значений в столбцах и их типах в таблице.
+ проверяем число непустых значнений
+ Выводим основную статистическую информацию о столбцах.
2. __Преобразование данных__
+ создаем с помощью функции-преобразования новый признак **"Образование"**, который должен иметь 4 категории: "высшее", "неоконченное высшее", "среднее специальное" и "среднее".
+ создаем два новых признака **"Пол"** и **"Возраст"**
+ преобразуем признак **"Опыт работы"**
+ создаем отдельные признаки **"Город"**, **"Готовность к переезду"**, **"Готовность к командировкам"**
+ создадем признаки-мигалки для признаков **"Занятость"** и **"График"**
+ приводим данные об ожидаемой заработной платы к общему виду
3. **Исследование зависимостей в данных**
+ анализируем распределение признака **"Возраст"**
+ рассматриваем распределение признака **"Опыт работы (месяц)"**
+ анализируем распределение признака **"ЗП (руб)"**
+ строим диаграмму, которая показывает зависимость **медианной** желаемой заработной платы (**"ЗП (руб)"**) от уровня образования (**"Образование"**)
+ строим диаграмму, которая показывает распределение желаемой заработной платы (**"ЗП (руб)"**) в зависимости от города (**"Город"**)
+ строим **многоуровневую столбчатую диаграмму**, которая показывает зависимость медианной заработной платы (**"ЗП (руб)"**) от признаков **"Готовность к переезду"** и **"Готовность к командировкам"**
+ строим сводную таблицу, иллюстрирующую зависимость **медианной** желаемой заработной платы от возраста (**"Возраст"**) и образования (**"Образование"**)
+ строим **диаграмму рассеяния**, показывающую зависимость опыта работы (**"Опыт работы (месяц)"**) от возраста (**"Возраст"**)
4. Очистка данных
+ находим полные дубликаты и удаляем их
+ выводим информацию о пропусках
+ обрабатываем пропуски
+ производим ручную очистку данных
+ строим распределение признака **"Возраст"** в логорифмическом масштабе
+ находим выбросы с помощью метода z-отклонения и удаляем их из данных

[к оглавлению](оглавление)


### Результаты:  
Данные преобразованы к удобному виду, произведены исследование зависимостей и очистка данных

[к оглавлению](#оглавление)


### Выводы:  
Отработаны основные этапы работы с данными на примере датасета о резюме
[к оглавлению](#оглавление)