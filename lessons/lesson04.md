патчи к лекции - 


# Четвертое занятие

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [Разбор домашнего задания](https://drive.google.com/file/d/1rk7vfY9ydCtXVtuJJQ13n2equleJvbV1/view?usp=sharing)
**Коммиты:**
 - [`lesson04 HW03`]

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 1. [Работа со строками](https://drive.google.com/file/d/1vIfmI6idbLJWou8NatlTKgsgMT4U0tWB/view?usp=sharing)
**Коммиты:**
 - [`Lesson04 String`]

**Ресурсы:**
- [Строки в Java](https://urvanov.ru/2016/04/20/java-8-строки/)
- [Кодировка в Java](http://www.skipy.ru/technics/encodings.html)
- [Ошибки при использовании строк](http://www.skipy.ru/technics/strings.html)
- [Обработка строк в Java](https://habrahabr.ru/post/260767/)
- **Дополнительно:**
  - [StringBuilder vs StringBuffer](https://stackoverflow.com/questions/355089/difference-between-stringbuilder-and-stringbuffer?rq=1)
  - [String vs StringBuffer vs StringBuilder](https://www.journaldev.com/538/string-vs-stringbuffer-vs-stringbuilder)
  - [String literal pool](http://java67.blogspot.ru/2014/08/difference-between-string-literal-and-new-String-object-Java.html)

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 2. [Исключения](https://drive.google.com/file/d/1XcK9UZYCJWHPy-UZXK_xJduSloKXvR-p/view?usp=sharing)
**Коммиты:**
 - [`Lesson04 Exceptions`]

**Ресурсы:**
  - [Исключения (Exceptions)](http://proglang.su/java/exceptions)
  - [Статья про исключения](http://developer.alexanderklimov.ru/android/java/exception.php)
  - Про исключения также можно почитать в книге Джошуа Блоха - ["Java. Эффективное программирование"](https://www.ozon.ru/context/detail/id/21724143/)
  - [Конструктор](http://info.javarush.ru/javarush_articles/2015/12/04/Конструкторы-классов-Java-JDK-1-5-.html)
  - [Ключевые слова: this, super](http://info.javarush.ru/grishin/2015/03/31/Разница-между-ключевыми-словами-this-и-super-в-Java.html)
  - **Дополнительно:**
    - [Exceptions](https://docs.oracle.com/javase/tutorial/essential/exceptions/)
    - [Checked vs unchecked exception explanation](https://stackoverflow.com/questions/6115896/java-checked-vs-unchecked-exception-explanation)

![image](https://cloud.githubusercontent.com/assets/18701152/15581283/4c2f5348-2374-11e6-8fd2-e4de02d2c389.png)

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 3. [Reflection. Аннотации. Модульное тестирование](https://drive.google.com/file/d/1LDd3Ekmi9kn-12Fzxf7M0pOGX_Cvji1K/view?usp=sharing)
**Коммиты:**
 - [`Lesson04 Reflection and JUnit`]
 
**Ресурсы:**
 - [Java 8 аннотации](https://urvanov.ru/2016/03/30/java-8-аннотации/)
 - [Reflection для начинающих](https://youtu.be/XJQuBXWADZg) (youtube)
 - [Руководство по Java Reflection API](http://javadevblog.com/polnoe-rukovodstvo-po-java-reflection-api-refleksiya-na-primerah.html)
 - [Java Reflection Example Tutorial](https://www.journaldev.com/1789/java-reflection-example-tutorial)
 - **Дополнительно:**
   - [The Reflection API](https://docs.oracle.com/javase/tutorial/reflect/)
   - [What is reflection and why is it useful?](https://stackoverflow.com/questions/37628/what-is-reflection-and-why-is-it-useful)
> В нашем проекте Reflection используют JUnit и будут использовать библиотеки работы с XML и JSON
 - [Фреймворк для модульного тестирования JUnit](http://junit.org/)
 - [Тестирование с помощью JUnit (Test Case)](http://www.javenue.info/post/19)
 - [Тестирование кода Java с помощью фреймворка JUnit](https://www.youtube.com/watch?v=z9jEVLCF5_w) (youtube)

## Домашнее задание HW4
- Реализуйте тесты: `AbstractArrayStorageTest`, `ArrayStorageTest` и `SortedArrayStorageTest`
- В `MainReflection` сделайте вызов метода `toString` через отражение, и выведите результат

## ![error](https://cloud.githubusercontent.com/assets/13649199/13672935/ef09ec1e-e6e7-11e5-9f79-d1641c05cbe6.png) Подсказки по HW4
- `SortedArrayStorageTest` должен запускаться с `SortedArrayStorage`
- `ArrayStorageTest` c `ArrayStorage`
- тестировать правильность сортировки не надо
- логика реализации теста на переполнение массива (`StorageException`):
  - заполняем массив, но не вызываем у него переполнение
  - если исключение вылетит раньше, чем массив будет заполнен, то тест должен провалиться (см. [`Assert.fail()`](https://stackoverflow.com/questions/3869954/whats-the-actual-use-of-fail-in-junit-test-case))
  - если исключение вылетает, когда пытаемся добавить в полностью заполненный массив еще одно резюме - тест пройден
- добавьте конструктор в `AbstractArrayStorageTest`, который инициализирует `Storage storage`, а в наследниках добавьте конструкторы, которые будут вызывать `super()` с нужным хранилищем
