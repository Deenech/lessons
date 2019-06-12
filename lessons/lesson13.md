патчи к лекции - 


# Тринадцатое занятие

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [1. Базы данных. Реляционные СУБД. PostgreSQL](https://drive.google.com/file/d/1_F5t_wX0LTjpXaSLLvrSJeCKpSIVhmxd/view?usp=sharing)
**Коммиты:**

- [`Lesson13 Init DB`]

**Ресурсы:**
- [DB-Engines Ranking](http://db-engines.com/en/ranking)
- [Реляционная СУБД](https://ru.wikipedia.org/wiki/Реляционная_СУБД) (wiki)
- [Введение в базы данных](http://www.codenet.ru/progr/vbasic/vb_db/1.php)
- [Реляционные базы vs NoSQL](http://habrahabr.ru/post/103021). SQL. Денормализация. PK, FK, Cascade
- [PostgreSQL: надёжность](https://ru.wikipedia.org/wiki/PostgreSQL#Качество_исходного_кода)
- [Работа с базами данных из IDEA](https://habrahabr.ru/company/JetBrains/blog/204064)
- [IDEA Database tools](https://www.jetbrains.com/datagrip/features)
- [Как работает реляционная БД](https://habrahabr.ru/company/mailru/blog/266811)
- [SQL ключи во всех подробностях](https://habrahabr.ru/company/oleg-bunin/blog/348172)
- [Книги по postgreSQL](https://postgrespro.ru/education/books)
- [Интерактивная обучалка по postgreSQL](https://www.pgexercises.com/)

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [2. Конфигурирование данных в Java проекте](https://drive.google.com/file/d/162_BqWk7dopRL_58pv73Anr7WwzJksev/view?usp=sharing)
**Коммиты:**

[`Lesson13 properties`]

**Ресурсы:**

- [Properties sample](https://www.mkyong.com/java/java-properties-file-examples)
- Конфигурирование DB и каталога хранения  

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [3.Подключение DB в проект](https://drive.google.com/file/d/14fR_FYCGUNwP-RPVjecoxd7SrR0XoH1F/view?usp=sharing)
**Коммиты:**

[`Lesson13 SqlStorage`]

**Ресурсы:**

- [JDBC](http://ru.wikipedia.org/wiki/Java_Database_Connectivity)
- [JDBC Architecture](http://www.developersbook.com/jdbc/interview-questions/jdbc-interview-questions-faqs.php)
- [Книга: Семь баз данных за семь недель. Введение в современные базы данных и идеологию NoSQL](http://www.ozon.ru/context/detail/id/19383907)
- [Работа с базами данных с помощью JDBC драйвера](https://devcolibri.com/работа-с-бд-mysql-postgresql-с-помощью-jdbc-драйвера)
- [Уроки по JDBC](https://www.youtube.com/playlist?list=PLIU76b8Cjem5qdMQLXiIwGLTLyUHkTqi2)

### ![hw](https://cloud.githubusercontent.com/assets/13649199/13672719/09593080-e6e7-11e5-81d1-5cb629c438ca.png) Домашнее задание HW13
- Доделать `SqlStorage` без контактов и секций
- Для работы с DB надо в lib и проект добавить [драйвер базы данных](http://repo1.maven.org/maven2/org/postgresql/postgresql/42.2.1)
- Запустить `SqlStorageTest` (в `AbstractStorageTest` контакты и секции закоменченны), креденшелы к базе взять из `Config`
- Вынести общий код (`getConnection(), prepareStatement, catch SQLException`) в класс `SqlHelper`
