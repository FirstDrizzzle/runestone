..  Copyright (C)  Brad Miller, David Ranum, Jeffrey Elkner, Peter Wentworth, Allen B. Downey, Chris
    Meyers, and Dario Mitchell.  Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".

Упражнения для программирования
--------------------------------

#. Напишите рекурсивную функцию для вычисления факториала числа.

#. Напишите рекурсивную функцию для переворота списка.

#. Измените программу рекурсивного рисования дерева, используя одну из следующих идей:

- Изменяйте толщину ветвей таким образом, чтобы с уменьшением ``branchLen`` линии становились тоньше.

- Изменяейте цвет ветвей, чтобы при маленьких ``branchLen`` цвет линий был зелёным (как у листьев).

- Изменяейте угол поворота "черепашки", чтобы для каждой ветки он выбирался произвольным образом из некоторого интервала. Например, используйте углы между 15-ю и 45-ю градусами. Поэкспериментируйте, чтобы улучшить внешний вид дерева.

- Рекурсивно изменяйте ``branchLen`` таким образом, чтобы вместо заданной величины, из неё каждый раз вычиталось произвольное число из некоторого интервала.

Если вы воплотите все эти идеи, то получите весьма реалистично выглядящее дерево.

#. Найдите или придумайте алгоритм для рисования фрактальных гор. Подсказка: одним из возможных методов снова будет использование треугольников.

#. Напишите рекурсивную функцию для вычисления последовательности Фибоначчи. Как её производительность соотносится с итеративной версией?

#. Напишите решение для ханойской башни, используя три стека для хранения дисков.

#. Используя графический модуль ``turtle``, напишите рекурсивную программу, рисующую кривую Гильберта. 

#. Используя графический модуль ``turtle``, напишите рекурсивную программу, рисующую снежинку Коха.

#. Напишите программу для решения слудеющей задачи: у вас есть два кувшина - на четыре и три галлона. Но ни на одном из них нет маркировки. Также имеется насос, с помощью которого можно набирать воду. Как получить ровно два галлона в четырёхгаллоновом кувшине?

#. Обобщите программу выше таким образом, чтобы параметры вашего решения включали размер каждого кувшина и итоговое количество воды, которое нужно оставить в наибольшем из них.

#. Напишите программу для решения следующей задачи: три миссионера и три каннибала подошли к берегу реки, возле которого привязана лодка, вмещающая только двух человек. Каждому нужно перебраться на другой берег, чтобы продолжить путешествие. Однако, если на каком-нибудь из берегов каннибалов окажется больше, чем миссионеров, то миссионеры будут съедены. Найдите такую последовательность перевозок, чтобы все безопасно оказались на другом берегу реки.

#. Измените программу ханойской башни, используя модуль ``turtle`` для анимации перемещения дисков. Подсказка: вы можете создать несколько "черепашек" и придать им форму прямоугольников.

#. Треугольник Паскаля - это треугольник из чисел, расположенных в шахматном порядке таким образом, что 

   .. math::
      a_{nr} = {n! \over{r! (n-r)!}}

Это выражение имеет биномиальный коэффициент. Вы можете построить треугольник Паскаля, складывая два числа, лежащие выше текущего по диагоналям. Пример треугольника Паскаля:

   ::

                         1
                       1   1
                     1   2   1
                   1   3   3   1
                 1   4   6   4   1

Напишите программу, печатающую треугольник Паскаля. Она должна иметь параметр, задающий количество строк в треугольнике.

#. Предположим, вы учёный-информатик и вор произведений искусства в одном лице. Вы проникли в художественную галерею, но всё, что у вас есть с собой для переноски украденного - это рюкзак, вместимостью в *W* фунтов произведений искусства. Для каждой ценности из галереи вы знаете её стоимость и вес. Напишите динамическую функцию, которая поможет вам максимизировать прибыль. Вот аналогичная задача, с которой можно начать: допустим, ваш рюкзак выдерживает вес в 20 фунтов и есть следующие пять предметов:

:: 
   
        предмет   вес      стоимость
          1        2           3
          2        3           4
          3        4           8
          4        5           8
          5        9          10

#. Эта задача называется "о расстоянии между строками" и используется во многих исследовательских областях. Предположим, вы хотите трансформировать слово "algorithm" в слово "alligator". Можно копировать буквы из одного слова в другое (стоимость 5 единиц), удалять буквы (стоимость 20 единиц) или вставлять дополнительные буквы (стоимость 20 единиц). Общая стоимость трансформации одного слова в другое используется программами проверки орфографии для выдачи в качестве предположения близких друг к другу слов. Используя технику динамического программирования, разработайте алгоритм, дающий вам наименьшее расстояние между любыми двумя словами.

.. disqus::
