патчи к лекции - 


# Четырнадцатое занятие

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [Разбор Домашнего Задания-13](https://drive.google.com/file/d/1WietUfgcONm5UxEArqCbhLRdg6dpMPiS/view?usp=sharing)
[см. коммит Lesson14 HW13]

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [1. JOIN](https://drive.google.com/file/d/1ZwPKDLsdJlHW0dzFZTMEoFwQXkJofU45/view?usp=sharing)
[см. коммит Lesson14 JOIN]
- <a href="http://www.skillz.ru/dev/php/article-Obyasnenie_SQL_obedinenii_JOIN_INNER_OUTER.html">LEFT, RIGHT, INNER JOIN</a>
- [SQL Join](https://www.youtube.com/watch?v=EHvzvwAv7RU&index=1&list=PLY7PmJJFH5nT-lbFKxfbp3rw5BBuq5Azo) (youtube)
- Добавляем в `SqlStorage` контакты

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [2. Транзакции](https://drive.google.com/file/d/1Ni1ENxAItEpaKt_ACsevSI3dmrC9ZJSQ/view?usp=sharing)
[см. коммит Lesson14 Transaction_Batch]
- <a href="http://ru.wikipedia.org/wiki/Транзакция_(информатика)">Транзакция. ACID.</a> <a href="https://ru.wikipedia.org/wiki/Уровень_изолированности_транзакций">Уровни изоляции транзакций.</a>
- <a href="http://www.osp.ru/pcworld/2009/07/9708191/">Уровни изоляции транзакций в SQL</a>
- Добавляем в `SqlStorage` транзакции
- Batch execute.

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [3. Установка/запуск Tomcat](https://drive.google.com/file/d/1dqWbWBIP_FAnumkKyhP_m0RzJS_QGhTb/view?usp=sharing)
- Скачать и установить <a href="http://tomcat.apache.org/download-80.cgi">Tomcat 8</a>. Устанавливать лучше простым копированием из архива в каталог (в том числе и для unix). Следите чтобы в пути не было пробелов и национальных букв.
- Для доступа к <a href="http://localhost:8080/manager">Tomсat Manager</a> добавьте в конфигурацию Tomcat `TOMCAT_HOME\conf\tomcat-users.xml` права:
```
<user username="tomcat" password="tomcat" roles="tomcat,manager-gui,admin-gui"/>
```
- Запуск из `TOMCAT_HOME\bin\`: `catalina.bat start`
 
## Домашнее задание HW14
- Закончить реализацию `SqlStorage` с контактами
- Выделить общие части <a href="https://ru.wikipedia.org/wiki/Don%E2%80%99t_repeat_yourself">( DRY )</a>
