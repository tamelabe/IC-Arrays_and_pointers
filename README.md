# Arrays and pointers

## Quest 1. Sort & memory.

Создана программа src/sort.c, ожидающая на вход в stdin массив длиной 10 из целых чисел и выводящую этот же массив, но уже отсортированный по возрастанию. Выделены функции чтения, сортировки и вывода массива отдельно. Использован пузырьковый метод сортировки. Передача массива в функцию осуществляется по указателю. В случае ошибки выводится "n/a".

| Входные данные | Выходные данные |
| ------ | ------ |
| 4 3 9 0 1 2 100 2 7 -1 | -1 0 1 2 2 3 4 7 9 100 |

## Quest 2. Several arrays.

Изменена программа src/key9part1.c так, чтобы она принимала на вход длину массива и массив целых чисел. В качестве выхода она выводит в stdout сумму четных элементов массива и новый сформированный массив из элементов старого, на которые делится нацело подсчитанная ранее сумма. Передача массива в функцию осуществляется по указателю. Максимальный размер входного массива - 10. В случае ошибки и отстутствии четных элементов выводится "n/a".

| Входные данные | Выходные данные |
| ------ | ------ |
| 10<br/>4 3 9 0 1 2 0 2 7 -1 | 8<br/>4 1 2 2 -1 |

## Quest 4. Cyclic shift.

Создана программа src/cycle_shift.c, ожидающая на вход число `n`, массив `A` из `n` целых чисел и число `c`, на которое все элементы массива сдвигаются влево циклично. При этом, при отрицательном значении `c` сдвиг происходит вправо по массиву. На вывод подается измененный массив. Передача массива в функцию осуществляется по указателю. Максимальный размер входного массива - 10. В случае ошибки выводится "n/a".

| Входные данные | Выходные данные |
| ------ | ------ |
| 10<br/>4 3 9 0 1 2 0 2 7 -1<br/>2 | 9 0 1 2 0 2 7 -1 4 3 |

## Quest 5. Arbitrary-precision arithmetic.

Изменена программа src/key9part2.c так, чтобы она возвращала результат сложения и разности двух очень больших чисел, переданных программе на вход в виде массивов. Максимальная длина числа - 100 элементов типа int. Вводимые целые числа представляют собой десятичные цифры. В случае если вычитаемое больше уменьшаемого, в разности выводится "n/a". В случае ошибки выводится "n/a".

| Входные данные | Выходные данные |
| ------ | ------ |
| 1 9 4 4 6 7 4 4 0 7 3 7 0 9 5 5 1 6 1<br/>2 9 | 1 9 4 4 6 7 4 4 0 7 3 7 0 9 5 5 1 9 0<br/>1 9 4 4 6 7 4 4 0 7 3 7 0 9 5 5 1 3 2 |
| 0 1 0<br/>0 0 1 | 1 1<br/>9 |
