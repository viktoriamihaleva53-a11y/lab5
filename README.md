# Домашнее задание к работе 5

## Условие задачи
Создать программу вычисления указанной величины.
Результат проверить при заданных исходных значениях.
<img width="418" height="97" alt="image" src="https://github.com/user-attachments/assets/d4e4509a-b11e-4e4d-a295-8beca7e482d7" />


## 1. Алгоритм и блок-схема

### Алгоритм
1. **Начало**
2. Задать исходные данные:
   - `x` = 14.26; 
   - `y` = -1.22;
   - `z` = 3.5e-2;
3. Вычислить значение указанной величины t:
   - `t` = (2.0 * cos(x - PI / 6.0)) / (0.5 + sin(y) * sin(y)) *
    (1.0 + (z * z) / (3.0 - (z * z) / 5.0));
4. Выводим результат вычисления:
   - printf("Результат вычисления:\n");
printf("t = %.6f\n", t);
5. **Конец**

### Блок-схема
<img width="332" height="1124" alt="image" src="https://github.com/user-attachments/assets/390c67ca-614e-4200-8aa2-511be476b499" />


## 2. Реализация программы
#include <stdio.h>
#include <math.h>
#include <locale.h>

#define PI 3.14159265358979323846

int main() 
{
    setlocale(LC_ALL, "RUS");
    double x = 14.26;
    double y = -1.22;
    double z = 3.5e-2;

    double t = (2.0 * cos(x - PI / 6.0)) / (0.5 + sin(y) * sin(y)) *
        (1.0 + (z * z) / (3.0 - (z * z) / 5.0));

    printf("Исходные данные: \n");
    printf("x = %.2f\n", x);
    printf("y = %.2f\n", y);
    printf("z = %.2e\n\n", z);
    printf("Результат вычисления:\n");
    printf("t = %.6f\n", t);

    return 0;
}

## 3. Результаты работы программы

<img width="268" height="158" alt="image" src="https://github.com/user-attachments/assets/a332b250-d072-404b-9cfa-17d5db4b3596" />



