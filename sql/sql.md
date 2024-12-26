SQL works on CRUD operations (Create, Read, Update, Delete)
SQL is a langauge
SQL stands for Structured Query langauge
SQL is a RDBMS : Relation database managment System
SQL is supported by -

1. MySQL
2. MSSWL Server
3. Oracle
4. IBM
   We are gonna use MYSQL because it is a opensourse
   MySQL is mostly used by Meta & Adobe

Major difference in SQL and MYSQL
Query Language | Mysql iyself a RDBMS
Way to access Data | CRUd operation are done on it using SQL

Create a database -
CREATE DATABASE db_name;

To work on that database -
USE db_name;

To create a table -
CREATE TABLE table_name ();

To insert values into table -
INSERT INTO table_name VALUES(.....);

To Print table -
SELECT _ FROM student;
here the _ means all values from the table

SQL Datatypes -

    datatypes are the domain of the identfier or coloum or the constraints you are gonna create

Datatypes are as follows -
char - string 0-255, fixed size
varchar - string 0-255, varable datatype
-- major difference is that if we are using char then we are allocating the 255 space in memory
-- but if i am using varchar then i am using the varable space as per need to the limit of 255. when needed the space will be used or the required space will be only used

tinytext - string 0-255
text - string 0-65535
blob - string 0-65535 - binary large object - audio,files, video - data converted to bytes to store and again converted to normal form later
others are given in the image followed by :-
for more reference use w3school

Signed & Unsigned - when we take TINYINT the value is -128 to 127 is signed but when we know there are no negative values then we can do
unsigned TINYINT - which vaires from 0 to 255

command - CREATE TABLE tinyint(col int, col2 INT UNSIGNED);

advanced datatypes -

1. JSON - Javascript object notation(Col1 JSON)

types of commands in SQL

1. DDL - Database defination Langaguage - we define the relation schema (includes create , alter, drop, truncate, rename)

2. DRL/DQL - Data retrieval language or data query language - retrive data from tables (SELECT)

3. DML- Data modification language - used to perfrom modificatons in database - INSERT UPDATE DELETE

4. DCL - Data control language - to give authorities to the user -GRANT , REVOKE

5. TCL - Transaction Control Language - To manage Transactions done in the database - START TRANSACTION, COMMIT, ROLLBACK, SAVEPOINT - these are the atomic commands - its ether complete or not complete nothing in middle - like setof setps will complete nor not

Managing DB - DDL

1. CREATE DATABASE IF NOT EXISTS db_name
2. USE db_name{needed to choose the database on which we have to work on , switching between databases}
3. DROP DATABASE IF EXITS db_name {dropping databases - delete database}
4. SHOW DATABASE - list all the database in the server
5. SHOW TABLES - list all the tables in the selected databases

Two tables are connected with each other with the help of foreign key
these tables are called as childern table
and the one with primary key are known as the parent table or reference table

day 1 ----38:25 min/3:52:20 min----
