# Синтяева Елена Витальевна ИС/22-9-1

## Описание

Эта База данных используется для упарвления информацией о книгах, читателях, авторах и арендованных книгах.

![screen](screenshots/image2.png)



### Таблица Books
![screen](screenshots/image3.png)

 - booksID (INTEGER, PRIMARY KEY) - уникальный идентификатор книги
 - title (VARCHAR(50)) - название книги
 - price (INT) - цена книги
 - genre (VARCHAR(50)) - жанр книги
 - year_of_Publishing (DATE) - год издания книги
 - id_author (INT) - идентификатор автора книги, связан с таблицей Author по полю Author_id

 ### Таблица Taken_books:
![screen](screenshots/image4.png)

 - Taken_books_id (INTEGER, PRIMARY KEY) - уникальный идентификатор взятой книги
 - id_books (INT) - идентификатор книги, связан с таблицей Books по полю booksID
 - id_readers (INT) - идентификатор читателя, связан с таблицей Readers по полю readers_id
 - date_of_collection (TEXT) - дата получения книги
 - date_of_return (TEXT) - дата возврата книги
Связи: таблица связана с таблицами Books (по id_books) и Readers (по id_readers)


### Таблица Readers:
![screen](screenshots/image5.png)

 - readers_id (INTEGER, PRIMARY KEY) - уникальный идентификатор читателя
 - fio (VARCHAR(50)) - ФИО читателя
 - telephone (VARCHAR(50)) - телефон читателя
 - e_mail (VARCHAR(50)) - электронная почта читателя
 - date_of_birth (TEXT) - дата рождения читателя


### Таблица Author:
![screen](screenshots/image6.png)

 - Author_id (INTEGER, PRIMARY KEY) - уникальный идентификатор автора
 - fio (VARCHAR(50)) - ФИО автора
 - date_of_birth (TEXT) - дата рождения автора

## UNION
![screen](screenshots/image7.png)

## ORDER BY


## HAVING


## Вложеный Запрос

### SELECT

### WHERE


## Оконные функции 

### Агрегатные функции

### Ранжирующие функции

### Функции смещения

## JOIN 

### INNER JOIN

### LEFT JOIN

### RIGHT JOIN

### FULL OUTER JOIN 

### CROSS JOIN

## CASE 

## WITH