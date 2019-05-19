### Обработка последовательной файловой структуры на языке Си

Курсовая работа №6 по информатике, 2 семестр. Обработка последовательной файловой структуры на языке Си.

Вариант №4. Отпечатать список студентов, компьютеры которых нуждаются в апгрейде (более p устройств).


### Структура программы

structure.h -- заголовочный файл с реализацией структуры базы данных

io.h -- заголовочный файл с определением функций io.c

io.c -- содержит функции ввода, вывода и печати файлов

owner.h -- заголовочный файл с определением функций owner.c и реализацией списка владельцев

owner.c -- содержит функции создания списка, добавления элемента в список и уничтожения списка владельцев

execute.c -- выполнение задачи варианта (печать списка студентов, компьютеры которых нуждаются в апгрейде)

generate.c -- создание бинарного файла базы данных из текстового

print.c -- печать данных из бинарного файла

### Как использовать

Компиляция:
make

Создание двоичного файла с базой данных:
./generate file_from file_to

Печать базы данных из двоичного файла:
./print db_file

Печать списка студентов, компьютеры которых нуждаются в апгрейде (parametr -- минимальное количество компьютеров, нуждающихся в апгрейде, после которых происходит печать):
./execute db_file parameter