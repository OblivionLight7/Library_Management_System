A library management system is where you can view all the book present in your library, issue books to student, and do a lot more with it. It also has a portal for both employees and students.


Add a new books
Delete any book
View all the books in the library
Search for any particular subject to list all the books of that subject present in the library
Issue book to student Whereas in the Student Portal, they get rights to -
View all the books
Search for a specific one
You can either register as an Employee if you haven't done that yet or else just Login like any other portal, same applies to the Student portal. Once you register yourself you will be added to the serveside database from where your details will be fetched at the time of login.



NOTE --
Install these packages if you don't have them already in your system

tkinter - pip install tkinter
Pillow - pip install pillow
PyMySql - pip install pymysql

Create a database with any name and give your database name and password to-

main.py
AddBooks.py
DeleteBook.py
IssueBook.py
SearchBook.py
ViewBook.py
Create an Employee table with any name and add the following attributes to it - empid(PK),name,password,dept,doj,sal (Everything should be varchar) (Please keep the names of the attributes as given here)

Syntax - create table <tablename> (empid varchar(20) primary key,name varchar(30),password varchar(30),dept varchar(30),doj varchar(30),sal varchar(30));

Then go ahead and paste you employee table name to -

main.py
IssueBook.py
Create a Student table with any name and add the following attributes to it - rollno(PK),name,password,dept,sem,batch (Everything should be varchar) (Please keep the names of the attributes as given here)

Syntax - create table <tablename> (rollno varchar(20) primary key,name varchar(30),password varchar(30),dept varchar(30),sem varchar(30),batch varchar(30));

Then go ahead and paste you student table name to -

main.py
IssueBook.py
Create a books table with any name and add the following attributes to it - bid(PK),title,subject,author,status (Everything should be varchar) (Please keep the names of the attributes as given here)

Syntax - create table <tablename> (bid varchar(20) primary key,title varchar(30),subject varchar(30),author varchar(30),status varchar(30));

Then go ahead and paste you books table name to -

AddBooks.py
DeleteBook.py
IssueBook.py
SearchBook.py
ViewBooks.py
Create an issue table with any name and add the following attributes to it - bid(PK),issueto,issueby (Everything should be varchar) (Please keep the names of the attributes as given here)

Syntax - create table <tablename> (bid varchar(20) primary key,issueto varchar(30),issueby varchar(30));

Then go ahead and paste you issue table name to -

IssueBook.py

NOTE -- 

Please give all the passwords unique while registering as it fetches data on the basis of password and if more than one password is same it will throw an exception, also under the Role section when login if you are an employee type 'emp' else if you're a student type 'stu'