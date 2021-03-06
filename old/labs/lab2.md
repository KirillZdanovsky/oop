[Назад к описанию](../../README.md)

# Наследование и полиморфизм

Содержание:
- [Цель работы](#Цель-работы)
- [Теоретические сведения](#Теоретические-сведения)
- [Задание](#Задание)
  - [Вариант №1](#Вариант-№1)
  - [Вариант №2](#Вариант-№2)
  - [Вариант №3](#Вариант-№3)
- [Вопросы](#Вопросы)

## Цель работы

Научиться применять на практике механизмы наследования и полиморфизма, виртуальные функции и абстрактные классы.

## Теоретические сведения

Наследование – это механизм, посредством которого один класс может наследовать свойства другого.

Основная форма записи наследования:

```c++
class производный_клаcc : спецификатор_доступа базовый_класс
{
    // методы и поля класса
};
```

Спецификатором доступа может выступать одно из трех ключевых слов: `public`, `private`, `protected`. Спецификатор доступа позволяет ограничить доступ к наследуемым членам базового класса.

Виртуальная функция является членом класса. Она объявляется внутри базового класса и переопределяется в производном классе. Для того чтобы функция стала виртуальной, перед объявлением функции ставят ключевое слово `virtual`. Виртуальные функции используются для поддержания механизма динамического полиморфизма в `С++`.

## Задание

Используя принципы ООП, необходимо реализовать программу на языке программирования `С++` в зависимости от варианта:

```
Вариант = ((номер_студента_по_списку - 1) % 3) + 1
```

### Вариант №1

Реализовать программу для вычисления и сравнения площадей следующих фигур:
- эллипс,
- прямоугольник,
- треугольник.

В программе необходимо иметь хотя бы один абстрактный класс.

При запуске программа должна выполнять следующие действия:
1. создать две случайные фигуры,
2. задать фигурам случайные размеры,
3. вывести информацию о фигурах,
4. рассчитать площади фигур,
5. сравнить площади фигур, вывести названия большей фигуры.

Пример вывода:

```yaml
Треугольник: ширина=4 высота=2
Прямоугольник: ширина=5 высота=1
Прямоугольник больше Треугольника (5>4)
```

### Вариант №2

Реализовать программу, содержащую следующие классы:
- цистерна,
- вагон для перевозки автомобилей,
- вагон для перевозки леса,
- пассажирский вагон,
- вагон-ресторан.

В программе необходимо иметь хотя бы один абстрактный класс.

При запуске программа должна выполнять следующие действия:
1. создавать N (от 5 до 20) случайных вагонов (поезд),
2. рассчитать суммарный вес поезда (всех вагонов),
3. отобразить состав поезда.

Пример вывода:

```yaml
Вес: 42100 кг.
Состав: .[Ресторан].[Пассажиры].[Цистерна].[Лес].[Лес].[Лес].
```

### Вариант №3

Используя принципы ООП реализовать программу, содержащую следующие классы:
- вывод четных чисел,
- вывод нечетных чисел,
- вывод положительных чисел,
- вывод отрицательных чисел.

В программе необходимо иметь хотя бы один абстрактный класс.

При запуске программа должна выполнять следующие действия:
1. создать случайный класс для вывода чисел,
2. создать массив из N (от 10 до 20) случайных положительных и отрицательных чисел,
3. вывести исходный массив на экран,
4. вывести исходный массив с помощью случайного класса для вывода чисел.

Пример вывода:

```yaml
Массив: 10 -33 131 812 313 -113 -1 -24 13 44 52
Вывод отрицательных чисел: -33 -113 -1 -24
```

## Вопросы

1. Что такое наследование?
2. Чем виртуальный метод отличается от чистого виртуального метода?
3. Что такое полиморфизм?
4. Что такое абстрактный класс?
5. Возможности указателей базовых и абстрактных классов?