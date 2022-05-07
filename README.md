# sber-virtual-internship
Проект с виртуальной стажировки STUDRE x СБЕР. Функционал:
1. Парсинг из CSV файла в объектную модель (+ вывод)
2. Сортировка по одному и двум параметрам (компоратор, лямбда выражения)
3. Поиск объекта по максимальному значению поля
4. Подсчёт количества объектов с одинаковым значением поля

## Запуск и компиляция
###  Компиляция
```
mvn clean install assembly:single
```

### Запуск
```
java -jar sber-virtual-internship.jar par1 par2 par3 par4
```
par1 (Вывод):
1 - Вывод записей из CSV файла в консоль;
0 - Отключает указанный функционал

par2 (Сортировка):
1 - Сортировка городов по наименованию. Вариант реализации - лямбда-выражения;
2 - Сортировка городов по наименованию. Вариант реализации - компаратор;
3 - Сортировка городов по федеральному округу и наименованию. Вариант реализации - компаратор;
0 - Отключает указанный функционал

par3 (Поиск объекта по максимальному значению поля):
1 - Поиск индекса (id) города с наибольшим количеством населения. Вариант реализации: перебор массива;
2 - Поиск индекса (id) города с наибольшим количеством населения. Вариант реализации: stream().max(), компоратор;
0 - Отключает указанный функционал

par4:
1 - Поиск количества городов в разрезе регионов. Вариант реализации: конструкция if;
2 - Поиск количества городов в разрезе регионов. Вариант реализации: лямбда-выражения;
0 - Отключает указанный функционал


