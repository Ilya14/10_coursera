# 10_coursera

## Описание

Скрипт собирает информацию о курсах на Курсере и
выгружает ее в xlsx-файл. Если какая-либо информация отсутствует, то
в соответствующей ячейке в файле результата будет
указано "No information".

## Использование

Скрипт принимает следующие обязательные параметры:

* xlsx_file_name - имя xlsx-файла

* count - количество курсов

Пример:
```sh
$ python3.5 ./coursera.py data.xlsx 3
```

Для получения справки можно использовать аргументы -h или --help:

```sh
$ python3.5 ./coursera.py -h
usage: coursera.py [-h] xlsx_file_name count

The script obtains Coursera courses information and unloads it 
to the xlsx-file

positional arguments:
  xlsx_file_name  xlsx-file name
  count           Courses count

optional arguments:
  -h, --help      show this help message and exit
```

## Пример

Ниже приведен пример использования скрипта и его вывод:
```sh
$ python3.5 ./coursera.py data.xlsx 5
[1/5] Loading from https://www.coursera.org/learn/gamification
[2/5] Loading from https://www.coursera.org/learn/missing-data
[3/5] Loading from https://www.coursera.org/learn/vital-signs
[4/5] Loading from https://www.coursera.org/learn/modern-art-ideas
[5/5] Loading from https://www.coursera.org/learn/evolvinguniverse
Courses information is saved to the file "data.xlsx"!
```