# Лабораторная работа №1
Ноутбук lab1.ipynb

Неочевидные моменты (на мой взгляд) прокомментированы в ноутбуке

# Лабораторная работа №2
Ноутбук lab2.ipynb

## Ход выполнения
1. Загружены данные с постами из StackOverflow и языками программирования из википедии
2. В таблице постов оставлены столбцы _CreationDate, _ViewCount, _Tags, Даты постов преобразованы в годы с помощью функции year(), отброшены строки с отсутствующими данными, отфильтрованы строки вне предела [2010, 2020]
4. Строковое значение _Tags преобразовано в список строк, с помощью explode каждый тэг вынесен в отдельную строку
5. Объединены таблицы постов и языков, отброшены строки с тегом, отсутствующеми в таблице языков
6. Таблица постов сгруппирована по годам и именам языков, просуммировано число просмотров
7. С помощью window языки отсортированы по просмотрам в рамках одного года, в каждом году взяты первые 10 языков
8. Результат сохранен в отчет с форматом .parquet
