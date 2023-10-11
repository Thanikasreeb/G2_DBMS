# EXP NO 1: DATA DEFINITION LANGUGE COMMANDS IN RDBMS
# AIM:
To create a student database and execute DDL queries using SQL.

# DDL (Data Definition Language)
DDL or Data Definition Language actually consists of the SQL commands that can be used to define the database schema. 
It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database. 
DDL is a set of SQL commands used to create, modify, and delete database structures but not data. These commands are normally not used by a general user, 
who should be accessing the database via an application.

# List of DDL commands:
CREATE: This command is used to create the database or its objects (like table, index, function, views, store procedure, and triggers). DROP: This 
command is used to delete objects from the database. 
ALTER: This is used to alter the structure of the database. 
TRUNCATE: This is used to remove all records from a table, including all spaces allocated for the records are removed. 
RENAME: This is used to rename an object existing in the database.

# Query:
# 1) Create a table student with the following fieds rollno,name,age,address,phoneno.
# SQL QUERY:
```
CREATE TABLE students(
    rollno numeric(5),name char(50),age numeric(5),
    address varchar(100),
    phoneno numeric(10)
    );
```

# OUTPUT:
![image](https://github.com/Thanikasreeb/G2_DBMS/assets/119557910/cdc158de-3dd0-4ea7-9edc-a9b5623e94cd)

# 2) Change the above student table by adding another attribute department
# SQL QUERY:
```
ALTER TABLE students ADD Department char(10);
```
# OUTPUT:
![image](https://github.com/Thanikasreeb/G2_DBMS/assets/119557910/d26200f1-0559-400d-8a7a-714632a48157)

# 3) Drop the student table
# SQL QUERY:
```
DROP TABLE students;
```
# OUTPUT:
![image](https://github.com/Thanikasreeb/G2_DBMS/assets/119557910/8935c91f-5b21-4e81-a0b5-431b61efc12c)

# 4) Delete the student table using truncate keyword
# SQL QUERY:
```
TRUNCATE TABLE students;
```
# OUTPUT:
![image](https://github.com/Thanikasreeb/G2_DBMS/assets/119557910/53869258-16e0-4d9d-834b-e36a186350d6)

# SQL QUERY:
```
ALTER TABLE students RENAME TO mystudents;
```
# OUTPUT:
![image](https://github.com/Thanikasreeb/G2_DBMS/assets/119557910/0a15cc89-bc3a-4192-bbb1-4e51faa0fb72)

# RESULT:
Thus a student database has been created and DDL queries are executed successfully




