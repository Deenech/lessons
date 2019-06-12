патчи к лекции - 


# Седьмое занятие

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [Разбор домашнего задания](https://drive.google.com/file/d/1EFGauuE1FeBH76une9chjfNJsoIc1MY1/view?usp=sharing)
**Коммиты:**
- [`Lesson07_HW06 test refactoring`]
- [`Lesson07_HW06 add fullName`]
- [`Lesson07_HW06 getAllSorted`]
- [`Lesson07_HW06 mapStorage`]

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [1. Параметризация. Стирание типов](https://drive.google.com/file/d/1GtvZseb1qwOoN6gTMfvWdIhfZAj2kcwo/view?usp=sharing)
**Коммиты:**
- [`Lesson07 generic`]

**Ресурсы:**
- [Дженерики (Java, обучающая статья)](http://www.quizful.net/post/java-generics-tutorial)
- [Обобщения (Generic)](http://developer.alexanderklimov.ru/android/java/generic.php)
- [Ограничения](http://docs.oracle.com/javase/tutorial/java/generics/restrictions.html)
- **Дополнительно**
  - [Java Generics Example Tutorial](https://www.journaldev.com/1663/java-generics-example-method-class-interface)

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [2. Логирование](https://drive.google.com/file/d/1EmWXXlUPVDubzf7Nxp7-nBqDOIk1WZW3/view?usp=sharing)
**Коммиты:**
- [`Lesson07 logging`]

**Ресурсы:**
- [Log4J (Apache logging)](https://logging.apache.org/)
- [Java Logging API - Tutorial](http://www.vogella.com/tutorials/Logging/article.html)
- [Логирование в Java / quick start](https://habrahabr.ru/post/130195/)
- [Ведение лога приложения](http://skipy.ru/useful/logging.html)
- [Java Logging: история кошмара](http://habrahabr.ru/post/113145/)

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [3. Синглтон. Enum](https://drive.google.com/file/d/1iMViwf5hQixUAzHapcmzRoCSkJyZzLzl/view?usp=sharing)
**Коммиты:**
- [`Lesson07 enum`]

**Ресурсы:**
- [Одиночка (шаблон проектирования)](https://ru.wikipedia.org/wiki/Одиночка_(шаблон_проектирования))
- [Перечисляемые типы (enum) в Java](http://easy-code.ru/lesson/enum-types-java)

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [Домашнее задание:](https://drive.google.com/file/d/1fiU2Pq5gnZNWdfLwsu6K8HX-MlllYOMh/view?usp=sharing)
[Доменный объект](https://ru.wikipedia.org/wiki/Доменный_объект)

- Начните выполнение ДЗ с рисования UML-диаграммы и покажите ее наставнику
- Сделать объектную модель резюме (диаграмма и классы). [**Образец резюме**](https://javawebinar.github.io)
  - Resume - главный класс. Делать только классы, включаемые в Resume (тип [отношения](https://github.com/ichimax/Java-Interview-Questions/blob/master/Questions/1.%20OOP.md#Типы-отношений-между-классами) - композиция)
  - Схожие по структуре и функциональности сущности делаем одним классом
  - Модель максимально упрощаем, и храним в ней только необходимые данные, а также функционал для вывода и редактирования резюме
  - В модели резюме должны быть представлены контакты и следующие секции:
    - PERSONAL("Личные качества")
    - OBJECTIVE("Позиция")
    - ACHIEVEMENT("Достижения")
    - QUALIFICATIONS("Квалификация")
    - EXPERIENCE("Опыт работы")
    - EDUCATION("Образование")
  - В секциях Достижения и Квалификация хранить список строк
  - Учесть в классах модели, что обработка резюме (вывод в html, сохранение, чтение) будет происходить следующим образом:
обработка `fullName`, цикл обработки по контактам, цикл обработки по секциям (для секций использовать полиморфизм, как для фигур: круг, квадрат...)
  - При добавлении / удалении новых видов контактов (например домашний телефон) или разделов изменения в коде (и БД) должны быть минимальны
- **ПРОВЕРЬТЕ свою модель: создайте класс ResumeTestData с методом main, а в нем объект `Resume` и заполните все его разделы данными, взятыми из [**Образца резюме**](https://javawebinar.github.io)**  
- **Не размещайте в AbstractStorageTest код, связанный с заполнением резюме данными. Делайте это в ResumeTestData**

#### Инструменты для рисования UML-диаграмм:

- [Generate class diagram in IntelliJ IDEA](http://stackoverflow.com/questions/8942751/use-intellij-to-generate-class-diagram#26926334) ([Help: working with Diagrams](https://www.jetbrains.com/help/idea/2016.1/working-with-diagrams.html?origin=old_help))
- Нарисовать и сфотографировать
- [Online: www.draw.io](http://www.draw.io)
- [yEd - Graph Editor](https://www.yworks.com/)
