# Домашнее задание к занятию "`Работа с данными (DDL/DML)`" - `Сайфиев Денис`


Задание можно калибровать как в любой IDE, так и в командной строке.

### Задание 1

1.1. Поднимите чистый инстанс MySQL версии 8.0+. Можно использовать локальный сервер или контейнер Docker.

1.2. Сделайте учётную запись sys_temp.

1.3. Выполните запрос на получение списка пользователей в базе данных. (скриншот)

1.4. Дайте все права для пользователя sys_temp.

1,5. Выполните запрос на получение списка прав для пользователя sys_temp. (скриншот)

1.6. Переподключитесь к базе данных от имени sys_temp.

Для смены типа аутентификации с sha2 воспользуйтесь запросом:

ALTER USER 'sys_test'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';
1.6. По ссылке https://downloads.mysql.com/docs/sakila-db.zip скачайте дамп базы данных.

1.7. Восстановите дамп в исходных данных.

1.8. При работе в IDE сформируйте ER-диаграмму полученной базы данных. При работе в командной строке воспользуйтесь командой для получения всех таблиц баз данных. (скриншот)

Результатом работы должны быть скриншоты графических заданий, а также простота со всеми запросами.

### Решение 1

![1.1.](https://github.com/DenioSa/DDL-DML/blob/82eb753599dbe11f181548478cd0590a4cdf7cc7/1.1..bmp)
![1.2.](https://github.com/DenioSa/DDL-DML/blob/82eb753599dbe11f181548478cd0590a4cdf7cc7/1.2..bmp)
![1.3.](https://github.com/DenioSa/DDL-DML/blob/82eb753599dbe11f181548478cd0590a4cdf7cc7/1.3..bmp)
![1.4.](https://github.com/DenioSa/DDL-DML/blob/82eb753599dbe11f181548478cd0590a4cdf7cc7/1.4..bmp)
![1.5.](https://github.com/DenioSa/DDL-DML/blob/82eb753599dbe11f181548478cd0590a4cdf7cc7/1.5..bmp)
![1.6.](https://github.com/DenioSa/DDL-DML/blob/82eb753599dbe11f181548478cd0590a4cdf7cc7/1.6..bmp)
![1.7.](https://github.com/DenioSa/DDL-DML/blob/82eb753599dbe11f181548478cd0590a4cdf7cc7/1.7..bmp)
![1.8.](https://github.com/DenioSa/DDL-DML/blob/82eb753599dbe11f181548478cd0590a4cdf7cc7/1.8..bmp)
![1.9.](https://github.com/DenioSa/DDL-DML/blob/82eb753599dbe11f181548478cd0590a4cdf7cc7/1.9..bmp)


### Задание 2

Составьте таблицу, используя любой текстовый редактор или Excel, в которой должно быть два столбца: во-первых, должно быть название таблицы восстановленной базы, во-вторых, название первичных ключей этих таблиц. Пример: (скриншот/текст)

Название таблицы           | Название первичного ключа
customer                    customer_id
_______________________________________________________       
actor                      | actor_id
address                    | address_id
category                   | category_id
city                       | city_id
country                    | country_id
customer                   | customer_id
film                       | film_id
film_actor                 | actor_id, film_id
film_category              | film_id, category_id
film_text                  | film_id
inventory                  | inventory_id
language                   | language_id
payment                    | payment_id
rental                     | rental_id
staff                      | staff_id
store                      | store_id
   
