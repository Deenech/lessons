патчи к лекции - 


# Пятнадцатое занятие

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [Разбор Домашнего Задания-14](https://drive.google.com/file/d/1j7d-pUvgUwGdepqVLtMxa1E-8M4SZh2T/view?usp=sharing)
[см. коммит Lesson15 HW14]

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [1. HTML, Tomcat](https://drive.google.com/file/d/1R0buUyNmolXlb0_nYcBdAC9rd6RbyRsN/view?usp=sharing)
[см. коммит Lesson15 web]

- <a href="http://java-course.ru/student/book1/servlet/">Протокол HTTP</a>. Смотрим <a href="http://topjava.herokuapp.com/">демо приложение<a/> в Chrome -> Инструменты разработчика
- Добавление в проект Web Facet. web.xml. Постороение/cтруктура WAR. Статические ресурсы.
- Настройка и деплой в Tomcat. Tomcat manager.
- Запуск Tomcat из IDEA. Динамическое обновление без передеплоя.

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [2. Сервлеты](https://drive.google.com/file/d/1KEC-_tTuVVUSEyRjxGC4yVfYjWWfqs2A/view?usp=sharing)
[см. коммит Lesson15 static_content]

[см. коммит Lesson15 servlets]

- <a href="http://devcolibri.com/как-создать-servlet-полное-руководство/">Создаем Servlet</a>. Параметры. Кодировка. 
- Дополнительно:
    - <a href="http://stackoverflow.com/questions/3106452/how-do-servlets-work-instantiation-shared-variables-and-multithreading">How do servlets work?</a>
    - <a href="http://www.intuit.ru/studies/courses/569/425/lecture/9683">Язык программирования Java: введение в сетевое программирование</a>
    - <a href="http://www.intuit.ru/studies/courses/1102/134/info">Основы работы с HTML</a>
    - <a href="http://ru.html.net/tutorials/html/">Учебник HTML</a>
    - [Ссылки по HTML, JavaScript, CSS](https://github.com/JavaOPs/topjava#html-javascript-css)

## Домашнее задание HW15
- Сделать реализацию `SqlStorage.getAllSorted` через 2 отдельных запроса: отдельно резюме и отдельно контакты.
- Добавить в реализацию `SqlStorage` и в базу секции (кроме `OrganizationSection`). Для `ListSection` склеиваем строки через `\n`.
- Сделать отображение таблицы резюме в сервлете (табл resume, т.е. только uuid и fullName).
  - <a href="http://www.webremeslo.ru/html/glava4.html">HTML таблицы</a>
