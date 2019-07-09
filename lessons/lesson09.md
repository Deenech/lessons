патчи к лекции - 


# Девятое занятие

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [Разбор Домашнего Задания](https://drive.google.com/file/d/1QmglZtKBufgjvxi9pQ6HM73fMZ5v1aIU/view?usp=sharing)
>Для создания и заполнения данными резюме из класса AbstractStorageTest используйте ResumeTestData. Не делайте это в AbstractStorageTest!

**Коммиты:**
- [`Lesson09 HW08`]

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [1. Ввод/вывод](https://drive.google.com/file/d/1wcnCTcq15do9UUJeO8ULU198RszvUpaA/view?usp=sharing)

**Ресурсы:**
- <a href="http://www.intuit.ru/studies/courses/16/16/lecture/27133">Пакет java.io</a>
- <a href="http://ru.wikipedia.org/wiki/Декоратор_(шаблон_проектирования)">Паттерн Декоратор</a>.
- <a href="http://www.intuit.ru/studies/courses/16/16/lecture/27133?page=4">Классы Reader и Writer.</a>
 
## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [2. Сериализация](https://drive.google.com/file/d/1IWCMyy0oq1K4JqaEMhGkagRxoRZZcnfT/view?usp=sharing)
**Коммиты:**
- [`Lesson09 ObjectStreamStorage`]

**Ресурсы:**
- <a href="http://www.intuit.ru/studies/courses/16/16/lecture/27133?page=3">Сериализация объектов (serialization)</a>
- Реализация Storage используя <a href="https://habrahabr.ru/post/60317/">сериализацию</a>.
- Сериализация: [1](https://www.youtube.com/watch?v=dBcqizwOWLg), [2](https://www.youtube.com/watch?v=nr4_JRKCGBU) (youtube)
 
## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [3. NIO](https://drive.google.com/file/d/1I_xlcpoY2LagC-mV4_kiY1W-HCSXgNwD/view?usp=sharing)
**Коммиты:**
- [`Lesson09 AbstractPathStorage`]

**Ресурсы:**
- <a href="http://www.quizful.net/post/java-nio-tutorial">NIO Java 7</a>
- <a href="https://habrahabr.ru/post/269667/">Чтения строк из файла</a>

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) [4. Основы Java 8 Stream API](https://drive.google.com/file/d/1jiDIKY3rsopFTfujWfRtDQiNC0wuJQDV/view?usp=sharing)
**Ресурсы:**
- <a href="https://annimon.com/article/2778">Потоки</a>

## Домашнее задание
- Сделать рекурсивный вывод каталогов и файлов с отступами
- Реализовать `ObjectStreamPathStorage` (через `java.nio.file.Path`) и добавить `ObjectStreamPathStorageTest`
- Сделать реализации `Storage` сохранения в файл через `File` и `Path` с возможностью выбора стратегии сериализации (посмотрите на [паттерн стратегия](https://refactoring.guru/ru/design-patterns/strategy)). Кроме сохранения через `ObjectOutputStream/ObjectInputStream` у нас будут еще несколько вариантов сериализации. Сделать тесты для тестирования сохранения через `ObjectOutputStream/ObjectInputStream` для `File` и `Path`.
