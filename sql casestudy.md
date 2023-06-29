# Case Study
+ create table book_table(book_id int,title varchar(20),author varchar(20),publisher varchar(20),publication_year date,isbn int,genre varchar(10),availability boolean,primary key(book_id));

+ select * from book_table;

+ create table borrowers_table(borrower_id int,name varchar(30),address varchar(50),phone_number numeric,email varchar(20),primary key(borrower_id));

+ select * from borrowers_table;

+ create table loans_table(loan_id int,book_id int,borrower_id int,date_borrowed date,due_date date,date_returned date,foreign key(book_id) references book_table(book_id),foreign key(borrower_id) references borrowers_table(borrower_id));

+ select * from loans_table;

+ create table reservations_table(reservation_id int,book_id int,borrower_id int,date_reserved date,date_needed date,status varchar(10),primary key(reservation_id), foreign key(book_id) references book_table(book_id),foreign key(borrower_id) references borrowers_table(borrower_id));

+ select * from reservations_table;