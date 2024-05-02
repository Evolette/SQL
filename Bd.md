```
CREATE TABLE Books (
booksID INTEGER PRIMARY key,
title VARCHAR(50),
price INT,
genre VARCHAR(50),
year_of_Publishing DATA,
id_author INT,
FOREIGN KEY(id_author) REFERENCES Author(ID));

CREATE TABLE Taken_books (
Taken_books_id INTEGER PRIMARY key,
id_books INT,
id_readers INT,
date_of_collection TEXT(50),
date_of_return TEXT(50),
FOREIGN KEY(id_books) REFERENCES Books(ID),
FOREIGN KEY(id_readers) REFERENCES Readers(ID));

CREATE TABLE Readers (
readers_id INTEGER PRIMARY key,
fio VARCHAR(50),
telephon VARCHAR(50),
e_mail VARCHAR(50),
date_of_birth TEXT(50));

CREATE TABLE Author (
Author_id INTEGER PRIMARY key,
fio VARCHAR(50),
date_of_birth TEXT(50)
title_of_book VARCHAR(50)                                                                                                                                                                                                                         
```
