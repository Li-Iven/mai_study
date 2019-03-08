### Методы оптимизации ###

Написанная на коленке прога, реализующая:
* классический метод
* метод градиентного спуска
* метод наискорейшего спуска (два разных выбора шага)
* метод градиентного спуска для плохо обусловленных функций
* метод покоординатного спуска
* метод Гаусса-Зейделя


### Использование ###

```
main.py [--methods=#] [--max-iter=#] [--output=<filename>]

  Флаги:
    methods=#
        Номера методов, которые нужно использовать. По умолчанию используются все методы.

        1 -- Классический метод
        2 -- Метод градиентного спуска
        3 -- Метод наискорейшего спуска с 1 выбором шага
        4 -- Метод наискорейшего спуска с 3 выбором шага
        5 -- Метод градиентного спуска для плохо обусловленных функций
        6 -- Метод покоординатного спуска
        7 -- Метод Гаусса-Зейделя

    Пример:
        --methods=1,3

    max-iter=#
        Максимальное количество итераций для каждого метода. По умолчанию 10000.
    Пример:
        --max-iter=5

    output=<filename>
        Запись вывода в файл.
    Пример:
        --output=log.txt
```