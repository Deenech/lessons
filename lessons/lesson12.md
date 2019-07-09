патчи к лекции - 


# Двенадцатое занятие

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [Разбор Домашнего Задания-11](https://drive.google.com/file/d/1m1S0qkZFgR72jeq-w8YipB3gAzFjydyv/view?usp=sharing)
[см. коммит Lesson12 HW11]

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [Concurrency](https://drive.google.com/file/d/1HY1LF_ILWgLicWfcAk2GD3lt-oeD5ueV/view?usp=sharing)
[см. коммит Lesson12 Concurrency]

- <a href="http://habrahabr.ru/company/luxoft/blog/157273/">Обзор java.util.concurrent.*</a></li>
- <a href="https://en.wikipedia.org/wiki/Compare-and-swap">Compare-and-swap</a>
- <a href="https://habrahabr.ru/post/277669/"> Справочник по синхронизаторам java.util.concurrent.*</a>
- <a href="http://articles.javatalks.ru/articles/17">Использование ThreadLocal переменных</a>

>  Замечания по видео:

    ThreadLocal<SimpleDateFormat> DATE_FORMAT = new ThreadLocal<SimpleDateFormat>() {
       @Override
       protected SimpleDateFormat initialValue() {
            return new SimpleDateFormat("dd.MM.yyyy HH:mm:ss");
       };
    };

можно написать через лямбду:

    ThreadLocal.withInitial(() -> new SimpleDateFormat("dd.MM.yyyy HH:mm:ss"));

А лучше использовать потокобезопасный `DateTimeFormatter` Java 8 Time API:

    DateTimeFormatter.ofPattern("dd.MM.yyyy HH:mm:ss");


## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [Разбор Домашнего Задания-10](https://drive.google.com/file/d/1l_DWFq_mHPCJ1P2bw9KIXRuE_NxAtXTK/view?usp=sharing)
[см. коммит Lesson12 HW10]

## Домашнее задание:
- <a href="http://java-course.ru/begin/postgresql">Установить PostgreSQL</a>
- Посмотреть на реляционные базы данных и SQL:
  - <a href="http://www.codenet.ru/progr/vbasic/vb_db/1.php">Введение в базы данных</a>
  - <a href="http://www.intuit.ru/studies/courses/5/5/info">Основы SQL</a>
- Java 8 Streams:
    1) реализовать метод через стрим `int minValue(int[] values)`.  
Метод принимает массив цифр от 1 до 9, надо выбрать уникальные и вернуть минимально возможное число, составленное из этих уникальных цифр. Не использовать преобразование в строку и обратно. Например {1,2,3,3,2,3} вернет 123, а {9,8} вернет 89

    2)  реализовать метод `List<Integer> oddOrEven(List<Integer> integers)`
если сумма всех чисел нечетная - удалить все нечетные, если четная - удалить все четные. Сложность алгоритма должна быть O(N). 
Optional - решение в один стрим.
