# Репозиторий для занятий по Си
## Теория
1. [Функции](theory/functions.md)
2. [Конструкция switch-case](theory/switch.md)

## Задачи

### Занятие 19 марта
1. [Задача про меню](practice/19.03.23/simple_menu.c) 

#### Домашнее задание
1. Сделать задачу #1 из прошлого дз (про рисование символами в консоли)
   > Вводим два числа А и Б (длина и ширина прямоугольника). В консоли должен нарисоваться прямоугольник из символа `#`;
   > ``` 
    > 2 3 \
    > ### \
    > ### \
    ```

2. Улучшить [задачу про меню](practice/19.03.23/simple_menu.c): 
   1. Вынести обработку через switch в отдельную функцию menu_logic;
   2. Вынести основной цикл (бесконечный) в отдельную функцию menu_runner. 
   > Таким образом, в main должен остаться только вызов menu_runner.

3.  Написать программу, которая дает словесное описание оценок. 
   > 1,2 - неуд;
   > 3 - удов;
   > 4-хор; 
   > 5- отл.
   Требования:
   1. Использовать switch
   2. Вынести в отдельную функцию convert_and_print mark основную логику программы.
   3. Число (оценку) считывать в main и передавать в функцию как параметр. 
   4. Для некорректной оценки выводить сообщение в консоль
    > вспоминаем default в switch

4. Написать калькулятор. Реализовать действия +-*/ и возведение в степень (код взять из прошлого дз). 
   1) Считывание выражения из консоли: scanf(“%i%c%i”, &a, &operator, &b);
   2) Написать отдельные функции с реализацией для каждого математического действия.
   3) Все оптации возвращают double 
   4) Использовать switch
   5) Калькулятор вынести в функцию `calcucate`, которая принимает **a**, **operator**, **b** и возвращает результат операции
   6) В main остается: чтение и парсинг выражения (см. п.(1)), вызов функции калькулятора (см. п.5), вывод результата в виде «a+b=17383”

 5.  Написать функцию, которая по координатам х,у выводит номер четверти. Если точка лежит на оси возвращать 0. 
   > Сделать через if else \
   > В main() только: чтение x и y, вызов функции и печать результата