# String_Calculator
Можно ввести любое выражение, например: 57.16 + 2^3^1.5 - (365.78^sin(sqrt(5,243) + 11,78) + ctg(8.45+99)) / (5! + 8 - 11) и вычислить его.

Калькулятор был написан на чистом языке Си, почти без использования стандартных библиотечных функций. Точнее, из стандартной библиотеки использовалась только функция pow (), потому что моя реализация этой функции еще недостаточно точна. Остальные функции и алгоритмы разработаны и написаны самостоятельно. Все алгоритмы имеют либо линейную сложность (при условии, что длина числа не зависит от длины выражения), либо логарифмическую сложность (это функции для вычисления тригонометрических функций). Калькулятор "понимает" скобки, возведение в степень, унарный минус, факториал, экспоненциальный ввод, извлечение корня любого порядка, прямые и обратные тригонометрические функции (при реализации которых использовался метод половинного деления остатка, как в алгоритме двоичного поиска). Последовательное возведение в степень в виде 2^2^2^2 понимается правоассоциативно, как 2^(2^(2^2)), то есть 2^16. Программа игнорирует пробелы и отлавливает ошибки ввода. В качестве аргумента тригонометрической функции может быть передано не только действительное число, но и выражение вида 3.147+5.56-1.45*7+55.8/7.1159, не содержащее скобок.

Примеры тестов:

8.6871*0.5^(-0.189)*0.0237^ (-0.0147) + sqrt(5,12.69*8+32/0.897) + sin(98.7)

8.6871*0.5^(-0.189)*0.0237^ (-0.0147) + sqrt(5,12.69*8+32/0.897) + sin(98.7)+ ctg(sqrt(10,1024))

(sin(90) + sin(30) + cos(55.8) + 15.68)/12.35^(ctg(86.7)-sin(4.5))

(sin(90) + sin(30) + cos(55.8) + 15.68)/12.35^(ctg(86.7)  + sin(4.5))

((sin(90) + sin(30) + cos(55.8) + 15.68)/12.35^(ctg(86.7)-sin(4.5)))^(sin(90) * sin(30)^2) 

3.24e3 * 0.125^(-1.568)

348e-3 + 5*(sin(46.8 + 5125.67)/0.867 + 1.57)

-12.2257*1.25/0.88^5.556*1.125   +  45.248*0.987*1.789^5.457/0.897^0.55  -479.214*0.1297

(((sin(90) + sin(30) + cos(55.8) + 15.68)/12.35^(ctg(86.7)-sin(4.5)))^(sin(90) + sin(30) + 1))^(arcsin(0.5)^cos(60)^2)




