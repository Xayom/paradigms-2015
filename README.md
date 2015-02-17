Тесты к курсу «Парадигмы программирования»
====

[Условия домашних заданий](http://www.kgeorgiy.info/courses/java-intro/homeworks.html)

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
