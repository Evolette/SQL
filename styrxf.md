# Синтяева Елена Витальевна ИС/22-9-1

## Описание

Эта База данных используется для упарвления информацией о книгах, читателях, авторах и арендованные книги.

![147](https://cdn.discordapp.com/attachments/1225378430086942720/1227237903030288534/147.png?ex=662d9c1d&is=662c4a9d&hm=f2cb54019357b0f61486c86a891fbb0afffdbf5ed4317ada63b29c2bc1a44a3b&)



### Таблица Books
![Фото](https://cdn.discordapp.com/attachments/1155576287969169439/1234407179206004788/image.png?ex=66309ec5&is=662f4d45&hm=2426b1bde8210e9a3346c807d8fc8e2e27b8ec5664cc8b7ce7b85da3245280cb&)

 - booksID (INTEGER, PRIMARY KEY) - уникальный идентификатор книги
 - title (VARCHAR(50)) - название книги
 - price (INT) - цена книги
 - genre (VARCHAR(50)) - жанр книги
 - year_of_Publishing (DATE) - год издания книги
 - id_author (INT) - идентификатор автора книги, связан с таблицей Author по полю Author_id

 ### Таблица Taken_books:
![Изображения](https://cdn.discordapp.com/attachments/1155576287969169439/1234407179206004788/image.png?ex=66309ec5&is=662f4d45&hm=2426b1bde8210e9a3346c807d8fc8e2e27b8ec5664cc8b7ce7b85da3245280cb&)

 - Taken_books_id (INTEGER, PRIMARY KEY) - уникальный идентификатор взятой книги
 - id_books (INT) - идентификатор книги, связан с таблицей Books по полю booksID
 - id_readers (INT) - идентификатор читателя, связан с таблицей Readers по полю readers_id
 - date_of_collection (TEXT) - дата получения книги
 - date_of_return (TEXT) - дата возврата книги
Связи: таблица связана с таблицами Books (по id_books) и Readers (по id_readers)


### Таблица Readers:
![image](https://cdn.discordapp.com/attachments/1155576287969169439/1234407245614420089/image.png?ex=66309ed5&is=662f4d55&hm=0485553aaea906a5c3a532cd1f5491858cda9d9a8660e1ed28c78e6644958bd5&)

 - readers_id (INTEGER, PRIMARY KEY) - уникальный идентификатор читателя
 - fio (VARCHAR(50)) - ФИО читателя
 - telephone (VARCHAR(50)) - телефон читателя
 - e_mail (VARCHAR(50)) - электронная почта читателя
 - date_of_birth (TEXT) - дата рождения читателя


### Таблица Author:
![image2](https://cdn.discordapp.com/attachments/1155576287969169439/1234407245614420089/image.png?ex=66309ed5&is=662f4d55&hm=0485553aaea906a5c3a532cd1f5491858cda9d9a8660e1ed28c78e6644958bd5&)

 - Author_id (INTEGER, PRIMARY KEY) - уникальный идентификатор автора
 - fio (VARCHAR(50)) - ФИО автора
 - date_of_birth (TEXT) - дата рождения автора

## UNION


## ORDER BY


## HAVING


## Вложеный Запрос:

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