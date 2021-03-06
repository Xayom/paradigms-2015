Тесты к курсу «Парадигмы программирования»
====

[Условия домашних заданий](http://www.kgeorgiy.info/courses/java-intro/homeworks.html)

Домашнее задание 6. Разбор выражений
---
 * *Базовая*
    * Реализовать интерфейс [Parser](java/expression/Parser.java)
    * [Исходный код тестов](java/expression/ParserTest.java)


Домашнее задание 5. Вычисление выражений
---
 * *Простая*
    * Реализовать интерфейс [DoubleExpression](java/expression/DoubleExpression.java)
    * [Исходный код тестов](java/expression/DoubleExpressionTest.java)
 * *Усложненная*
    * Реализовать интерфейс [TripleExpression](java/expression/TripleExpression.java)
    * [Исходный код тестов](java/expression/TripleExpressionTest.java)
 * *Базовая*
    * Реализовать интерфейс [Expression](java/expression/Expression.java)
    * [Исходный код тестов](java/expression/ExpressionTest.java)

Домашнее задание 4. Очередь на связном списке
---
 * *Простая*
    * Добавить в интерфейс очереди и реализовать метод
      `toArray`, возвращающий массив,
      содержащий элементы, лежащие в очереди в порядке
      от головы к хвосту
    * Исходная очередь должна остаться неизменной
    * Дублирования кода быть не должно
    * [Исходный код тестов](java/QueueToArrayTest.java)
    * [Откомпилированные тесты](artifacts/QueueToArrayTest.jar)
 * *Усложненная*
    * Добавить в интерфейс очереди и реализовать методы
        * `filter(predicate)` – создать очередь, содержащую элементы, удовлетворяющие 
            [предикату](https://docs.oracle.com/javase/8/docs/api/java/util/function/Predicate.html)
        * `map(function)` – создать очередь, содержащую результаты применения 
            [функции](https://docs.oracle.com/javase/8/docs/api/java/util/function/Function.html)
    * Исходная очередь должна остаться неизменной
    * Тип возвращаемой очереди должен соответствовать типу исходной очереди
    * Взаимный порядок элементов должен сохраняться
    * Дублирования кода быть не должно
    * [Исходный код тестов](java/FQueueTest.java)
    * [Откомпилированные тесты](artifacts/FQueueTest.jar)
 * *Базовая*
    * [Исходный код тестов](java/QueueTest.java)
    * [Откомпилированные тесты](artifacts/QueueTest.jar)

Домашнее задание 3. Очередь на массиве
---
Модификации
 * *Простая*
    * Реализовать метод `toArray`, возвращающий массив,
      содержащий элементы, лежащие в очереди в порядке
      от головы к хвосту.
    * [Исходный код тестов](java/ArrayQueueToArrayTest.java)
    * [Откомпилированные тесты](artifacts/ArrayQueueToArrayTest.jar)
 * *Усложненная*
    * Реализовать методы
        * `push` – добавить элемент в начало очереди
        * `peek` – вернуть последний элемент в очереди
        * `remove` – удалить последний элемент из очереди 
    * [Исходный код тестов](java/ArrayQueueDequeTest.java)
    * [Откомпилированные тесты](artifacts/ArrayQueueDequeTest.jar)
 * *Базовая*
    * [Исходный код тестов](java/ArrayQueueTest.java)
    * [Откомпилированные тесты](artifacts/ArrayQueueTest.jar)

Домашнее задание 2. Бинарный поиск
----
Модификации
 * *Простая*
    * Если в массиве `a` отсутствует элемент, равный `x`, то требуется
      вывести индекс вставки в формате, определенном в 
      [`Arrays.binarySearch`](http://docs.oracle.com/javase/8/docs/api/java/util/Arrays.html#binarySearch-int:A-int-).
    * Класс должен иметь имя `BinarySearchMissing`
    * [Исходный код тестов](java/BinarySearchMissingTest.java)
    * [Откомпилированные тесты](artifacts/BinarySearchMissingTest.jar)
 * *Усложненная*
    * Требуется вывести два числа: начало и длину диапазона элементов,
      равных `x`. Если таких элементов нет, то следует вывести
      пустой диапазон, у которого левая граница совпадает с местом
      вставки элемента `x`.
    * Не допускается использование типов `long` и `BigInteger`.
    * Класс должен иметь имя `BinarySearchSpan`
    * [Исходный код тестов](java/BinarySearchSpanTest.java)
    * [Откомпилированные тесты](artifacts/BinarySearchSpanTest.jar)
 * *Базовая*
    * [Исходный код тестов](java/BinarySearchTest.java)
    * [Откомпилированные тесты](artifacts/BinarySearchTest.jar)

Домашнее задание 1. Сумма чисел
----

Модификации
 * *Простая*
    * Входные данные помещаются в тип `long`
    * Класс должен иметь имя `SumLong`
    * [Исходный код тестов](java/SumLongTest.java)
    * [Откомпилированные тесты](artifacts/SumLongTest.jar)
 * *Усложненная*
    * Входные данные помещаются в тип `long`
    * На вход подаются десятичные и шестнадцатеричные числа
    * Шестнадцатеричные числа имеют префикс `0x`
    * Ввод регистронезависим
    * Класс должен иметь имя `SumLongHex`
    * [Исходный код тестов](java/SumLongHexTest.java)
    * [Откомпилированные тесты](artifacts/SumLongHexTest.jar)

Для того, чтобы протестировать исходную программу:

 1. Скачайте тесты ([SumTest.jar](artifacts/SumTest.jar))
 * Откомпилируйте `Sum.java`
 * Проверьте, что создался `Sum.class`
 * В каталоге, в котором находится `Sum.class` выполните команду 
    ```
       java -jar <путь к SumTest.jar>
    ```
	* Например, если `SumTest.jar` находится в текущем каталоге, выполните команду 
    ```
    	java -jar SumTest.jar
	```
    
Исходный код тестов: 

* [SumTest.java](java/SumTest.java), 
* [SumChecker.java](java/SumChecker.java)
