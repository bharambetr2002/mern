### SQL Notes

#### Basics of SQL
- **SQL works on CRUD operations** (Create, Read, Update, Delete).
- **SQL** stands for Structured Query Language.
- SQL is a **language** used for managing data in a relational database.
- **SQL is supported by RDBMS (Relational Database Management Systems)** like:
  1. MySQL
  2. MSSQL Server
  3. Oracle
  4. IBM DB2

We will focus on **MySQL** because:
- It is **open source**.
- Widely used by companies like Meta and Adobe.

#### Major Difference Between SQL and MySQL
| **SQL**                     | **MySQL**                    |
|-----------------------------|------------------------------|
| A query language            | A relational database system |
| Used for CRUD operations    | CRUD operations performed on it using SQL |

#### Basic Commands
1. **Create a Database**:
   ```sql
   CREATE DATABASE db_name;
   ```

2. **Select the Database to Work On**:
   ```sql
   USE db_name;
   ```

3. **Create a Table**:
   ```sql
   CREATE TABLE table_name (
       column_name data_type constraints
   );
   ```

4. **Insert Values into Table**:
   ```sql
   INSERT INTO table_name VALUES (value1, value2, ...);
   ```

5. **Retrieve Data from Table**:
   ```sql
   SELECT * FROM table_name;
   ```
   - `*` selects all columns from the table.

#### SQL Data Types
Data types define the **domain** and **constraints** of a column. Key data types include:

1. **Character Data Types**:
   - **`CHAR(n)`**: Fixed-length string (0-255 characters).
   - **`VARCHAR(n)`**: Variable-length string (0-255 characters).
     - **Difference**: `CHAR` allocates full memory for `n`, whereas `VARCHAR` uses only required space up to `n`.

2. **Text Data Types**:
   - **`TINYTEXT`**: Up to 255 characters.
   - **`TEXT`**: Up to 65,535 characters.
   - **`BLOB`**: Binary large object (e.g., audio, video, files).
     - Converts data to bytes for storage and back for use.

3. **Numeric Data Types**:
   - **Signed**: Allows negative and positive values (e.g., `-128` to `127` for `TINYINT`).
   - **Unsigned**: Allows only positive values (e.g., `0` to `255` for `TINYINT`).
     ```sql
     CREATE TABLE example (
         col1 TINYINT,
         col2 TINYINT UNSIGNED
     );
     ```

4. **Advanced Data Types**:
   - **`JSON`**: Stores data in JSON format.
     ```sql
     CREATE TABLE example (
         col1 JSON
     );
     ```

#### Types of SQL Commands
1. **DDL (Data Definition Language)**:
   - Defines schema: `CREATE`, `ALTER`, `DROP`, `TRUNCATE`, `RENAME`.

2. **DRL/DQL (Data Retrieval/Query Language)**:
   - Retrieves data: `SELECT`.

3. **DML (Data Manipulation Language)**:
   - Modifies data: `INSERT`, `UPDATE`, `DELETE`.

4. **DCL (Data Control Language)**:
   - Manages permissions: `GRANT`, `REVOKE`.

5. **TCL (Transaction Control Language)**:
   - Manages transactions: `START TRANSACTION`, `COMMIT`, `ROLLBACK`, `SAVEPOINT`.
   - Ensures atomicity (all or nothing execution).

#### Managing a Database
1. **Create a Database**:
   ```sql
   CREATE DATABASE IF NOT EXISTS db_name;
   ```

2. **Switch Between Databases**:
   ```sql
   USE db_name;
   ```

3. **Drop a Database**:
   ```sql
   DROP DATABASE IF EXISTS db_name;
   ```

4. **List All Databases**:
   ```sql
   SHOW DATABASES;
   ```

5. **List All Tables in Current Database**:
   ```sql
   SHOW TABLES;
   ```

#### Relationships in SQL
- **Primary Key**: Uniquely identifies each record in a table (Parent Table).
- **Foreign Key**: Connects two tables by referencing the primary key of another table (Child Table).

---

*Notes Updated: Continue from timestamp 38:25 min.*
