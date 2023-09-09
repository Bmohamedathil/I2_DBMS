# EXP NO 1: DATA DEFINITION LANGUGE COMMANDS IN RDBMS

## AIM:
To create a student database and execute DDL queries using SQL.


## DDL (Data Definition Language)
<div align="justify">
DDL or Data Definition Language actually consists of the SQL commands that can be used to define the database schema. It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database. DDL is a set of SQL commands used to create, modify, and delete database structures but not data. These commands are normally not used by a general user, who should be accessing the database via an application.
</div>
 
## List of DDL commands: 
<div align="justify">
CREATE: This command is used to create the database or its objects (like table, index, function, views, store procedure, and triggers).
DROP: This command is used to delete objects from the database.
ALTER: This is used to alter the structure of the database.
TRUNCATE: This is used to remove all records from a table, including all spaces allocated for the records are removed.
RENAME: This is used to rename an object existing in the database.
</div>

## Query:
### 1) Create a table student with the following fieds rollno,name,age,address,phoneno.

### SQL QUERY: 
```
CREATE TABLE students(rollno INT,name VARCHAR(100),age INT,address VARCHAR(100),phoneno VARCHAR(15));
```
### OUTPUT:
![image](https://github.com/Bmohamedathil/I2_DBMS/assets/119560261/a2fd0599-2192-4df1-b2e3-7870874e1066)

### 2) Change the above student table by adding another attribute department

### SQL QUERY: 
```
INSERT INTO students(rollno, name, age, address, phoneno) VALUES (1, 'John', 20, 'CHENNAI', '9153657854');
INSERT INTO students(rollno, name, age, address, phoneno) VALUES (2, 'SMITH', 25, 'TRICHY', '9746441548');
```
### OUTPUT:
![image](https://github.com/Bmohamedathil/I2_DBMS/assets/119560261/b0ca72b2-26eb-4917-a536-4e843ced5c2c)

### 3) Drop the student table
 
### SQL QUERY: 
```
DROP TABLE students;
```
### OUTPUT:
![image](https://github.com/Bmohamedathil/I2_DBMS/assets/119560261/4fd2555d-8baa-4ce4-bc9e-a50c7624483f)

### 4) Delete the student table using truncate keyword

### SQL QUERY: 
```
TRUNCATE TABLE mystudent;
```

### OUTPUT:

![image](https://github.com/Bmohamedathil/I2_DBMS/assets/119560261/181ee9bb-6446-45fe-920d-8157828a528a)

### 5) Rename the student table to mystudent

### SQL QUERY: 
```
ALTER TABLE students RENAME TO mystudent;
```
### OUTPUT:
![image](https://github.com/Bmohamedathil/I2_DBMS/assets/119560261/5cca9807-bb22-4070-8e8d-3f2068bcf4df)
