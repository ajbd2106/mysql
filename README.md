# mysql
MySQL Repository for training

## Homework 1
 - В рамках первого ДЗ была подготовлена виртуальная машина на базе **Ubuntu 20**, на которой был установлен **MySQL 8.0** и проведена его базовая настройка
 - Были установлены на рабочую ОС **Workbench**, **DBeaver** и настроены удаленные подключения к серверу MySQL
 - Скриншоты по результатам работы были добавлены в папку **topic1**

## Homework 2
 - В рамках второго ДЗ был подготовлен файл **.my.cnf**, благодаря которому можно запускать клиент mysql и mysqldump без указания логин/пароля
 - Была создана база данных example, в ней создана таблица users, состоящаю из двух столбцов - числового id и строкового name. Список команд представлен в файле **example.sql**. Результат команд представлен на скриншоте **example.png**
 - Был создан дамп базы данных example из предыдущего задания, содержимое дампа было развернуто в новую базу данных sample. Список команд для восстановления дампа представлен в файле **sample_restore.sql**. Результат выполнения дампа и восстановления представлен на скриншоте **sample.png**
 - Был создан дамп единственной таблицы help_keyword базы данных mysql, который содержит только первые 100 строк таблицы. Для этого необходимо выполнить команду - *mysqldump mysql help_keyword --where="1 limit 100" > mysql_help_keyword_100.sql*

## Homework 3
 - В рамках третьего ДЗ была создана структура БД **vk**. Все команды для ее создания представлены в файле **vk_create.sql**.
 - С использованием сервиса *http://filldb.info* были сгенерированы тестовые данные для всех таблиц. Дамп базы данных представлен в виде файла **vk.sql**. Для его загрузки достаточно создать базу данных с именем **vk** и выполнить команду *mysql vk < vk.sql*.
 - В базовом файле **vk_create.sql** были внесены изменения для колонки *size* в таблице *media*. Был добавлен флаг *UNSIGNED* ввиду того, что отрицательное значение неактуально для размера файла. 
