# MySQL
# Лекции https://pollen-attempt-4ac.notion.site/SQL-9072b1ca09f94e6fa3c588804919e1ae
# ДЗ_1
Урок 1. Установка СУБД, подключение к БД, просмотр и создание таблиц
Создайте таблицу с мобильными телефонами (mobile_phones), используя графический интерфейс. Заполните БД данными. Добавьте скриншот на платформу в качестве ответа на ДЗ
Необходимые поля таблицы:
    product_name (название товара),
    manufacturer (производитель),
    product_count (количество),
    price (цена). 
2. Выведите название, производителя и цену для товаров, количество которых превышает 2
3.  Выведите весь ассортимент товаров марки “Samsung”
4. (по желанию)* С помощью регулярных выражений найти:
	4.1. Товары, в которых есть упоминание "Iphone"
	4.2. Товары, в которых есть упоминание "Samsung"
	4.3.  Товары, в которых есть ЦИФРЫ
	4.4.  Товары, в которых есть ЦИФРА "8" 
	
# ДЗ_2
Урок 2. SQL – создание объектов, простые запросы выборки
* 1.Используя операторы языка SQL,
создайте таблицу “sales”. Заполните ее данными.Справа располагается рисунок к первому заданию.
id order_date count_product 
1 2022-01-01 156
2 2022-01-02 180
3 2022-01-03 21
4 2022-01-04 124
5 2022-01-05 341
* 2.Для данных таблицы “sales” укажите тип заказа в зависимости от кол-ва :
меньше 100 -Маленький заказ от 100 до 300 -Средний заказ больше 300 -Большой заказ
idзаказа Тип заказа 1 Средний заказ 2 Средний заказ 3 Маленький заказ 4 Средний заказ 5 Большой заказ
* 3.Создайте таблицу “orders”, заполните ее значениями
id employee_id amount order_status
1 e03 15.00 OPEN
2 e01 25.50 OPEN
3 e05 100.70 CLOSED
4 e02 22.18 OPEN
5 e04 9.50 CANCELLED
Выберите все заказы. В зависимости от поля order_status 
-- выведите столбец full_order_status: OPEN –«Order is in open state»; CLOSED -«Order is closed»; CANCELLED -«Order is cancelled»
* 4.Чем 0 отличается от NULL?

# ДЗ_3
Урок 3. SQL – выборка данных, сортировка, агрегатные функции
* Таблица staff для заданий
id firstname lastname post seniority salary age
1	Вася	Петров	Начальник	40	100000	60
2	Петр	Власов	Начальник	8	70000	30
3	Катя	Катина	Инженер	2	70000	25
4	Саша	Сасин	Инженер	12	50000	35
5	Иван	Иванов	Рабочий	40	30000	59
6	Петр	Петров	Рабочий	20	25000	40
7	Сидр	Сидоров	Рабочий	10	20000	35
8	Антон	Антонов	Рабочий	8	19000	28
9	Юрий	Юрков	Рабочий	5	15000	25
10	Максим	Максимов	Рабочий	2	11000	22
11	Юрий	Галкин	Рабочий 	3	12000	24
12	Людмила	Маркина	Уборщик	10	10000	49
* 1.Отсортируйте данные по полюзаработная плата (salary) в порядке: убывания; возрастания
* 2.Выведите 5 максимальных заработных плат (saraly)
* 3.Посчитайте суммарную зарплату (salary)по каждой специальности(роst)
* 4.Найдите кол-во сотрудников с специальностью (post)«Рабочий»в возрасте от 24 до 49 лет включительно.
* 5.Найдите количество специальностей
* 6.Выведите специальности, у которых средний возраст сотрудников меньше 30 лет
# ДЗ_4
Урок 4. SQL – работа с несколькими таблицами
Используя таблицы с семинаров:
1. Подсчитать общее количество лайков, которые получилипользователи младше 12 лет.
2. Определить кто больше поставиллайков(всего): мужчины или женщины.
3. Вывести всех пользователей, которые не отправляли сообщения.
4. (по желанию)*Пусть задан некоторый пользователь. Из всех друзей этого пользователя найдите человека, который больше всех написал ему сообщений.
# ДЗ_5
Урок 5. SQL – оконные функции
Для решения задач используйте базу данных lesson_4
(скрипт создания, прикреплен к 4 семинару).
1. Создайте представление, в которое попадет информация о пользователях (имя, фамилия, город и пол), которые не старше 20 лет.
2. Найдите кол-во, отправленных сообщений каждым пользователем и выведите ранжированный список пользователей, указав имя и фамилию пользователя, количество отправленных сообщений и место в рейтинге (первое место у пользователя с максимальным количеством сообщений) . (используйте DENSE_RANK)
3. Выберите все сообщения, отсортируйте сообщения по возрастанию даты отправления (created_at) и найдите разницу дат отправления между соседними сообщениями, получившегося списка. (используйте LEAD или LAG)
# ДЗ_6
