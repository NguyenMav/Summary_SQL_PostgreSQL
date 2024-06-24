# PostgreSQL Basics Cheat Sheet
![image](https://github.com/NguyenMav/Summary_SQL_PostgreSQL/assets/149219810/cf62454d-fe93-44e7-8de9-266661ba0038)

![image](https://github.com/NguyenMav/Summary_SQL_PostgreSQL/assets/149219810/28f19fc4-9627-49d3-8c0b-72b51a603c5d)

![image](https://github.com/NguyenMav/Summary_SQL_PostgreSQL/assets/149219810/e44c8697-e25e-4562-abf3-d23440a7ea9b)


# PostgreSQL Intermediate Cheat Sheet
![image](https://github.com/NguyenMav/Summary_SQL_PostgreSQL/assets/149219810/a7bca103-9b17-400f-a945-76baaff86906)

![image](https://github.com/NguyenMav/Summary_SQL_PostgreSQL/assets/149219810/db701c28-a23f-4f25-8232-bf0030e49b5c)


# PostgreSQL Advance Cheat Sheet
![image](https://github.com/NguyenMav/Summary_SQL_PostgreSQL/assets/149219810/058ab774-707a-4d8b-bba3-0ebbfd677a1c)

![image](https://github.com/NguyenMav/Summary_SQL_PostgreSQL/assets/149219810/a9fdc13d-b8e1-4858-b594-0bb78c0d339b)

# Complete PostgreSQL Keyword Explanations

## SQL Keywords and Functions Index
- [Data Types](#sql-data-types)
- [Data Query Language (DQL) Keywords](#data-query-language-dql-keywords)
  - [SELECT](#select)
  - [FROM](#from)
  - [WHERE](#where)
  - [GROUP BY](#group-by)
  - [HAVING](#having)
  - [ORDER BY](#order-by)
  - [JOIN](#join)
  - [UNION](#union)
  - [UNION ALL](#union-all)
  - [INTERSECT](#intersect)
  - [INTERSECT ALL](#intersect-all)
  - [LIMIT](#limit)
  - [OFFSET](#offset)
  - [DISTINCT](#distinct)
- [Data Manipulation Language (DML) Keywords](#data-manipulation-language-dml-keywords)
  - [INSERT](#insert)
  - [UPDATE](#update)
  - [DELETE](#delete)
  - [MERGE](#merge)
  - [CALL](#call)
  - [EXPLAIN PLAN](#explain-plan)
  - [LOCK TABLE](#lock-table)
  - [VALUES](#values)
  - [SET](#set)
- [Data Definition Language (DDL) Keywords](#data-definition-language-ddl-keywords)
  - [CREATE](#create)
  - [ALTER](#alter)
  - [DROP](#drop)
  - [TRUNCATE](#truncate)
  - [COMMENT](#comment)
  - [RENAME](#rename)
  - [ADD](#add)
  - [CONSTRAINT](#constraint)
  - [INDEX](#index)
  - [PRIMARY KEY](#primary-key)
  - [FOREIGN KEY](#foreign-key)
- [Data Control Language (DCL) Keywords](#data-control-language-dcl-keywords)
  - [GRANT](#grant)
  - [REVOKE](#revoke)
- [Transaction Control Language (TCL) Keywords](#transaction-control-language-tcl-keywords)
  - [COMMIT](#commit)
  - [ROLLBACK](#rollback)
  - [SAVEPOINT](#savepoint)
  - [SET TRANSACTION](#set-transaction)
- [JOIN Keywords](#join-keywords)
  - [INNER JOIN](#inner-join)
  - [LEFT JOIN](#left-join)
  - [RIGHT JOIN](#right-join)
  - [FULL JOIN](#full-join)
  - [CROSS JOIN](#cross-join)
  - [SELF JOIN](#self-join)
- [Aggregation Functions](#aggregation-functions)
  - [SUM](#sum)
  - [AVG](#avg)
  - [COUNT](#count)
  - [MIN](#min)
  - [MAX](#max)
- [Window Functions](#window-functions)
  - [ROW_NUMBER](#row_number)
  - [RANK](#rank)
  - [DENSE_RANK](#dense_rank)
  - [NTILE](#ntile)
  - [LAG](#lag)
  - [LEAD](#lead)
  - [FIRST_VALUE](#first_value)
  - [LAST_VALUE](#last_value)
  - [NTH_VALUE](#nth_value)
- [Numeric Functions](#numeric-functions)
  - [ABS](#abs)
  - [CEIL](#ceil)
  - [FLOOR](#floor)
  - [ROUND](#round)
  - [POWER](#power)
  - [SQRT](#sqrt)
  - [MOD](#mod)
- [Null Handling Functions](#null-handling-functions)
  - [COALESCE](#coalesce)
  - [NULLIF](#nullif)
  - [IS NULL](#is-null)
  - [IS NOT NULL](#is-not-null)
- [String Functions](#string-functions)
  - [UPPER](#upper)
  - [LOWER](#lower)
  - [INITCAP](#initcap)
  - [CONCAT](#concat)
  - [SUBSTRING](#substring)
  - [LENGTH](#length)
  - [TRIM](#trim)
  - [REPLACE](#replace)
- [Wildcard Characters](#wildcard-characters)
  - [% (Percent Sign)](#%)
  - [_ (Underscore)](#_)
- [Views](#views)
  - [CREATE VIEW](#create-view)
  - [ALTER VIEW](#alter-view)
  - [DROP VIEW](#drop-view)
  - [CREATE OR REPLACE VIEW](#create-or-replace-view)
- [PostgreSQL-Specific Keywords](#postgresql-specific-keywords)
  - [DO](#do)
  - [ILIKE](#ilike)
  - [PERFORM](#perform)
  - [SERIAL](#serial)
  - [UNLISTEN](#unlisten)
  - [VACUUM](#vacuum)
  - [RETURNING](#returning)
  - [ARRAY](#array)
  - [ANY and ALL](#any-and-all)
  - [pg_catalog](#pg_catalog)
  - [information_schema](#information_schema)
  - [pg_views](#pg_views)
  - [pg_tables](#pg_tables)
  - [pg_datatype](#pg_datatype)

### SQL Data Types

This table provides an overview of common SQL data types along with their descriptions. Adjust the data types and descriptions as per your specific SQL dialect and requirements.

| Data Type              | Description                                               |
|------------------------|-----------------------------------------------------------|
| `INT` or `INTEGER`     | Integer values, typically 32-bit signed integer in SQL.   |
| `SMALLINT`             | Small integer values, typically 16-bit signed integer.     |
| `BIGINT`               | Large integer values, typically 64-bit signed integer.     |
| `NUMERIC(precision, scale)` | Fixed-point number with specified precision and scale.  |
| `DECIMAL(precision, scale)` | Same as `NUMERIC`, with exact precision and scale.      |
| `FLOAT(p)` or `REAL`   | Floating-point number with specified precision.            |
| `DOUBLE PRECISION`     | Double precision floating-point number.                    |
| `CHAR(n)`              | Fixed-length character string with defined length `n`.     |
| `VARCHAR(n)` or `CHARACTER VARYING(n)` | Variable-length character string with maximum length `n`. |
| `TEXT`                 | Variable-length character string with no limit.            |
| `DATE`                 | Date value in YYYY-MM-DD format.                           |
| `TIME`                 | Time value in HH:MM:SS format.                             |
| `TIMESTAMP`            | Date and time value.                                       |
| `BOOLEAN`              | Boolean value (`TRUE` or `FALSE`).                         |
| `BINARY`               | Fixed-length binary string.                                |
| `VARBINARY`            | Variable-length binary string.                             |
| `BYTEA`                | Binary data (PostgreSQL).                                  |
| `ARRAY`                | Array of elements (PostgreSQL, MySQL).                     |
| `JSON`                 | JSON (JavaScript Object Notation) data (PostgreSQL, MySQL).|
| `UUID`                 | Universally unique identifier (PostgreSQL).                |
| `XML`                  | XML data type (SQL Server, PostgreSQL).                    |
| `GEOMETRY`             | Spatial data type (MySQL, PostgreSQL).                     |

### Data Query Language (DQL) Keywords

| Keyword       | Description |
|---------------|-------------|
| `SELECT`      | Retrieves data from a database. |
| `FROM`        | Specifies the table to retrieve data from. |
| `WHERE`       | Filters records based on a condition. |
| `GROUP BY`    | Groups records sharing a property for aggregation. |
| `HAVING`      | Filters groups based on a condition. |
| `ORDER BY`    | Sorts the result set. |
| `JOIN`        | Combines rows from two or more tables based on a related column. |
| `UNION`       | Combines the result sets of two or more `SELECT` statements. |
| `UNION ALL`   | Combines the result sets of two or more `SELECT` statements, including duplicates. |
| `INTERSECT`   | Returns the intersection of two or more `SELECT` statements. |
| `INTERSECT ALL` | Returns the intersection of two or more `SELECT` statements, including duplicates. |
| `DISTINCT`    | Returns only distinct (different) values. |
| `LIMIT`       | Specifies the number of records to return (or `TOP` in SQL Server). |
| `OFFSET`      | Specifies the starting point from which to return records. |

### `SELECT`
```sql
-- Retrieves all columns from a table
SELECT * FROM users;

-- Retrieves specific columns from a table
SELECT first_name, last_name FROM users;
```

### `FROM`
```sql
-- Specifies the table to retrieve data from
SELECT * FROM orders;
```

### `WHERE`
```sql
-- Filters records based on a condition
SELECT * FROM products WHERE price > 100;
```

### `GROUP BY`
```sql
-- Groups records sharing a property for aggregation
SELECT department, COUNT(*) as employee_count
FROM employees
GROUP BY department;
```

### `HAVING`
```sql
-- Filters groups based on a condition
SELECT department, COUNT(*) as employee_count
FROM employees
GROUP BY department
HAVING COUNT(*) > 5;
```

### `ORDER BY`
```sql
-- Sorts the result set
SELECT product_name, price FROM products
ORDER BY price DESC;
```

### `JOIN`
```sql
-- Combines rows from two tables based on a related column
SELECT orders.order_id, customers.customer_name
FROM orders
JOIN customers ON orders.customer_id = customers.customer_id;
```

### `UNION`
```sql
-- Combines the result sets of two SELECT statements
SELECT product_id, product_name FROM products
UNION
SELECT product_id, product_name FROM archived_products;
```

### `UNION ALL`
```sql
-- Combines the result sets of two SELECT statements, including duplicates
SELECT product_id, product_name FROM products
UNION ALL
SELECT product_id, product_name FROM archived_products;
```

### `INTERSECT`
```sql
-- Returns the intersection of two SELECT statements
SELECT product_id, product_name FROM products
INTERSECT
SELECT product_id, product_name FROM popular_products;
```

### `INTERSECT ALL`
```sql
-- Returns the intersection of two SELECT statements, including duplicates
SELECT product_id, product_name FROM products
INTERSECT ALL
SELECT product_id, product_name FROM popular_products;
```

### `DISTINCT`
```sql
-- Returns only distinct (different) values
SELECT DISTINCT department FROM employees;
```

### `LIMIT`
```sql
-- Specifies the number of records to return
SELECT * FROM orders
LIMIT 10;
```

### `OFFSET`
```sql
-- Specifies the starting point from which to return records
SELECT * FROM orders
LIMIT 10 OFFSET 20;
```

### Data Manipulation Language (DML) Keywords

| Keyword       | Description |
|---------------|-------------|
| `INSERT`      | Adds new rows of data to a table. |
| `UPDATE`      | Modifies existing data in a table. |
| `DELETE`      | Removes data from a table. |
| `MERGE`       | Merges two tables based on a condition. |
| `CALL`        | Executes a stored procedure. |
| `EXPLAIN PLAN`| Describes the execution plan of a query. |
| `LOCK TABLE`  | Locks a table for a transaction. |
| `VALUES`      | Specifies the values for an `INSERT` statement. |
| `SET`         | Specifies the column values for an `UPDATE` statement. |

### `INSERT`
```sql
-- Adds new rows of data to a table
INSERT INTO users (first_name, last_name, email)
VALUES ('John', 'Doe', 'john.doe@example.com');
```

### `UPDATE`
```sql
-- Modifies existing data in a table
UPDATE products
SET price = price * 1.1
WHERE category = 'Electronics';
```

### `DELETE`
```sql
-- Removes data from a table
DELETE FROM orders
WHERE order_date < '2023-01-01';
```

### `MERGE`
```sql
-- Merges two tables based on a condition
MERGE INTO target_table AS T
USING source_table AS S
ON T.id = S.id
WHEN MATCHED THEN
  UPDATE SET T.value = S.value
WHEN NOT MATCHED THEN
  INSERT (id, value) VALUES (S.id, S.value);
```

### `CALL`
```sql
-- Executes a stored procedure
CALL calculate_total_sales();
```

### `EXPLAIN PLAN`
```sql
-- Describes the execution plan of a query
EXPLAIN PLAN FOR
SELECT * FROM customers WHERE city = 'New York';
```

### `LOCK TABLE`
```sql
-- Locks a table for a transaction
LOCK TABLE orders IN SHARE MODE;
```

### `VALUES`
```sql
-- Specifies the values for an INSERT statement
INSERT INTO products (product_name, price)
VALUES ('Laptop', 1200);
```

### `SET`
```sql
-- Specifies the column values for an UPDATE statement
UPDATE employees
SET salary = salary * 1.05
WHERE department = 'Finance';
```

### Data Definition Language (DDL) Keywords

| Keyword       | Description |
|---------------|-------------|
| `CREATE`      | Creates a new table, view, or other database object. |
| `ALTER`       | Modifies an existing database object. |
| `DROP`        | Deletes an existing database object. |
| `TRUNCATE`    | Removes all rows from a table without logging individual row deletions. |
| `COMMENT`     | Adds a comment to a database object. |
| `RENAME`      | Renames a database object. |
| `ADD`         | Adds a new column to a table. |
| `CONSTRAINT`  | Adds a constraint to a column. |
| `INDEX`       | Creates an index on a table. |
| `PRIMARY KEY` | Defines a column as the primary key. |
| `FOREIGN KEY` | Defines a column as a foreign key. |

### `CREATE`
```sql
-- Creates a new table
CREATE TABLE users (
    user_id INT PRIMARY KEY,
    username VARCHAR(50) NOT NULL,
    email VARCHAR(100)
);

-- Creates a new view
CREATE VIEW active_users AS
SELECT * FROM users WHERE is_active = true;
```

### `ALTER`
```sql
-- Modifies an existing database object (e.g., table)
ALTER TABLE users
ADD COLUMN birth_date DATE;

-- Modifies an existing view (e.g., renaming)
ALTER VIEW active_users RENAME TO active_customers;
```

### `DROP`
```sql
-- Deletes an existing database object (e.g., table)
DROP TABLE products;

-- Deletes an existing view
DROP VIEW active_customers;
```

### `TRUNCATE`
```sql
-- Removes all rows from a table without logging individual row deletions
TRUNCATE TABLE logs;
```

### `COMMENT`
```sql
-- Adds a comment to a database object
COMMENT ON COLUMN users.username IS 'The username of the user';
```

### `RENAME`
```sql
-- Renames a database object
ALTER TABLE customers RENAME TO clients;
```

### `ADD`
```sql
-- Adds a new column to a table
ALTER TABLE orders
ADD COLUMN order_date DATE;
```

### `CONSTRAINT`
```sql
-- Adds a constraint to a column
ALTER TABLE employees
ADD CONSTRAINT fk_department
FOREIGN KEY (department_id)
REFERENCES departments(department_id);
```

### `INDEX`
```sql
-- Creates an index on a table
CREATE INDEX idx_product_name ON products(product_name);
```

### `PRIMARY KEY`
```sql
-- Defines a column as the primary key
ALTER TABLE orders
ADD PRIMARY KEY (order_id);
```

### `FOREIGN KEY`
```sql
-- Defines a column as a foreign key
ALTER TABLE order_details
ADD CONSTRAINT fk_order_id
FOREIGN KEY (order_id)
REFERENCES orders(order_id);
```

### Data Control Language (DCL) Keywords

| Keyword       | Description |
|---------------|-------------|
| `GRANT`       | Gives user permissions. |
| `REVOKE`      | Removes user permissions. |

### `GRANT`
```sql
-- Gives user permissions
GRANT SELECT, INSERT ON employees TO hr_user;
```

### `REVOKE`
```sql
-- Removes user permissions
REVOKE DELETE ON products FROM marketing_user;
```

### Transaction Control Language (TCL) Keywords

| Keyword           | Description |
|-------------------|-------------|
| `COMMIT`          | Saves all changes made in the current transaction. |
| `ROLLBACK`        | Reverts all changes made in the current transaction. |
| `SAVEPOINT`       | Sets a point within a transaction to which a rollback can occur. |
| `SET TRANSACTION` | Sets transaction properties. |

### `COMMIT`
```sql
-- Saves all changes made in the current transaction
COMMIT;
```

### `ROLLBACK`
```sql
-- Reverts all changes made in the current transaction
ROLLBACK;
```

### `SAVEPOINT`
```sql
-- Sets a point within a transaction to which a rollback can occur
SAVEPOINT before_update;

-- Rollback to a specific savepoint
ROLLBACK TO before_update;
```

### `SET TRANSACTION`
```sql
-- Sets transaction properties
SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
```

### JOIN Keywords

| Keyword       | Description |
|---------------|-------------|
| `INNER JOIN`  | Returns records with matching values in both tables. |
| `LEFT JOIN`   | Returns all records from the left table and matched records from the right table. |
| `RIGHT JOIN`  | Returns all records from the right table and matched records from the left table. |
| `FULL JOIN`   | Returns all records when there is a match in either left or right table. |
| `CROSS JOIN`  | Returns the Cartesian product of both tables. |
| `SELF JOIN`   | Joins a table with itself. |

### `INNER JOIN`
```sql
-- Returns records with matching values in both tables
SELECT orders.order_id, customers.customer_name
FROM orders
INNER JOIN customers ON orders.customer_id = customers.customer_id;
```

### `LEFT JOIN`
```sql
-- Returns all records from the left table and matched records from the right table
SELECT orders.order_id, customers.customer_name
FROM orders
LEFT JOIN customers ON orders.customer_id = customers.customer_id;
```

### `RIGHT JOIN`
```sql
-- Returns all records from the right table and matched records from the left table
SELECT orders.order_id, customers.customer_name
FROM orders
RIGHT JOIN customers ON orders.customer_id = customers.customer_id;
```

### `FULL JOIN`
```sql
-- Returns all records when there is a match in either left or right table
SELECT orders.order_id, customers.customer_name
FROM orders
FULL JOIN customers ON orders.customer_id = customers.customer_id;
```

### `CROSS JOIN`
```sql
-- Returns the Cartesian product of both tables
SELECT *
FROM orders
CROSS JOIN customers;
```

### `SELF JOIN`
```sql
-- Joins a table with itself
SELECT e1.employee_name AS employee, e2.employee_name AS manager
FROM employees e1
INNER JOIN employees e2 ON e1.manager_id = e2.employee_id;
```

### Aggregation Functions

| Function       | Description |
|----------------|-------------|
| `COUNT`        | Returns the number of rows that match a specified condition. |
| `SUM`          | Returns the total sum of a numeric column. |
| `AVG`          | Returns the average value of a numeric column. |
| `MIN`          | Returns the smallest value of a column. |
| `MAX`          | Returns the largest value of a column. |

### `COUNT`
```sql
-- Returns the number of rows that match a specified condition
SELECT COUNT(*) AS total_orders FROM orders;
```

### `SUM`
```sql
-- Returns the total sum of a numeric column
SELECT SUM(price) AS total_revenue FROM sales;
```

### `AVG`
```sql
-- Returns the average value of a numeric column
SELECT AVG(age) AS average_age FROM employees;
```

### `MIN`
```sql
-- Returns the smallest value of a column
SELECT MIN(salary) AS min_salary FROM employees;
```

### `MAX`
```sql
-- Returns the largest value of a column
SELECT MAX(salary) AS max_salary FROM employees;
```

### Window Functions

| Function       | Description |
|----------------|-------------|
| `ROW_NUMBER`   | Assigns a unique number to each row within the partition. |
| `RANK`         | Assigns a rank to each row within the partition. |
| `DENSE_RANK`   | Assigns ranks to rows without gaps. |
| `NTILE`        | Divides the result set into a specified number of roughly equal parts. |
| `LAG`          | Provides access to a row at a given physical offset prior to that position. |
| `LEAD`         | Provides access to a row at a given physical offset after that position. |
| `FIRST_VALUE`  | Returns the first value in an ordered set of values. |
| `LAST_VALUE`   | Returns the last value in an ordered set of values. |
| `NTH_VALUE`    | Returns the value at a specified position within an ordered set of values. |

### `ROW_NUMBER`
```sql
-- Assigns a unique number to each row within the partition
SELECT product_name, price,
       ROW_NUMBER() OVER (PARTITION BY category ORDER BY price DESC) AS row_num
FROM products;
```

### `RANK`
```sql
-- Assigns a rank to each row within the partition
SELECT department, employee_name, salary,
       RANK() OVER (PARTITION BY department ORDER BY salary DESC) AS dept_rank
FROM employees;
```

### `DENSE_RANK`
```sql
-- Assigns ranks to rows without gaps within the partition
SELECT department, employee_name, salary,
       DENSE_RANK() OVER (PARTITION BY department ORDER BY salary DESC) AS dept_dense_rank
FROM employees;
```

### `NTILE`
```sql
-- Divides the result set into a specified number of roughly equal parts
SELECT employee_name, salary,
       NTILE(4) OVER (ORDER BY salary DESC) AS salary_quartile
FROM employees;
```

### `LAG`
```sql
-- Accesses a row at a given physical offset prior to the current position
SELECT order_id, order_date, LAG(order_date, 1) OVER (ORDER BY order_date) AS previous_order_date
FROM orders;
```

### `LEAD`
```sql
-- Accesses a row at a given physical offset after the current position
SELECT order_id, order_date, LEAD(order_date, 1) OVER (ORDER BY order_date) AS next_order_date
FROM orders;
```

### `FIRST_VALUE`
```sql
-- Returns the first value in an ordered set of values
SELECT department, employee_name,
       FIRST_VALUE(salary) OVER (PARTITION BY department ORDER BY salary DESC) AS top_salary
FROM employees;
```

### `LAST_VALUE`
```sql
-- Returns the last value in an ordered set of values
SELECT department, employee_name,
       LAST_VALUE(salary) OVER (PARTITION BY department ORDER BY salary DESC ROWS BETWEEN UNBOUNDED PRECEDING AND UNBOUNDED FOLLOWING) AS max_salary
FROM employees;
```

### `NTH_VALUE`
```sql
-- Returns the value at a specified position within an ordered set of values
SELECT department, employee_name,
       NTH_VALUE(salary, 2) OVER (PARTITION BY department ORDER BY salary DESC) AS second_highest_salary
FROM employees;
```

### Numeric Functions

| Function       | Description |
|----------------|-------------|
| `ABS`          | Returns the absolute value of a number. |
| `CEIL`         | Returns the smallest integer greater than or equal to a number. |
| `FLOOR`        | Returns the largest integer less than or equal to a number. |
| `ROUND`        | Rounds a number to a specified number of decimal places. |
| `POWER`        | Returns the value of a number raised to the power of another number. |
| `SQRT`         | Returns the square root of a number. |
| `MOD`          | Returns the remainder of a division operation. |

### `ABS`
```sql
-- Returns the absolute value of a number
SELECT ABS(-10) AS absolute_value;
```

### `CEIL`
```sql
-- Returns the smallest integer greater than or equal to a number
SELECT CEIL(4.3) AS ceiling_value;
```

### `FLOOR`
```sql
-- Returns the largest integer less than or equal to a number
SELECT FLOOR(4.9) AS floor_value;
```

### `ROUND`
```sql
-- Rounds a number to a specified number of decimal places
SELECT ROUND(123.456, 2) AS rounded_value;
```

### `POWER`
```sql
-- Returns the value of a number raised to the power of another number
SELECT POWER(2, 3) AS power_value; -- Calculates 2^3
```

### `SQRT`
```sql
-- Returns the square root of a number
SELECT SQRT(25) AS square_root;
```

### `MOD`
```sql
-- Returns the remainder of a division operation
SELECT MOD(10, 3) AS modulus_value; -- Calculates 10 % 3
```

### Null Handling Functions

| Function       | Description |
|----------------|-------------|
| `COALESCE`     | Returns the first non-null value in a list. |
| `NULLIF`       | Returns null if the two arguments are equal. |
| `IS NULL`      | Checks if a value is null. |
| `IS NOT NULL`  | Checks if a value is not null. |

### `COALESCE`
```sql
-- Returns the first non-null value in a list
SELECT COALESCE(null_column, 'Default Value') AS replaced_value
FROM your_table;
```

### `NULLIF`
```sql
-- Returns null if the two arguments are equal
SELECT NULLIF(column1, column2) AS different_value
FROM your_table;
```

### `IS NULL`
```sql
-- Checks if a value is null
SELECT column_name
FROM your_table
WHERE column_name IS NULL;
```

### `IS NOT NULL`
```sql
-- Checks if a value is not null
SELECT column_name
FROM your_table
WHERE column_name IS NOT NULL;
```

### String Functions

| Function       | Description |
|----------------|-------------|
| `UPPER`        | Converts a string to uppercase. |
| `LOWER`        | Converts a string to lowercase. |
| `INITCAP`      | Converts the first letter of each word to uppercase and the rest to lowercase. |
| `CONCAT`       | Concatenates two or more strings. |
| `SUBSTRING`    | Extracts a substring from a string. |
| `LENGTH`       | Returns the length of a string. |
| `TRIM`         | Removes leading and trailing spaces from a string. |
| `REPLACE`      | Replaces all occurrences of a substring within a string. |

### `UPPER`
```sql
-- Converts a string to uppercase
SELECT UPPER('hello world') AS upper_string;
```

### `LOWER`
```sql
-- Converts a string to lowercase
SELECT LOWER('Hello World') AS lower_string;
```

### `INITCAP`
```sql
-- Converts the first letter of each word to uppercase and the rest to lowercase
SELECT INITCAP('hello world') AS initcap_string;
```

### `CONCAT`
```sql
-- Concatenates two or more strings
SELECT CONCAT(first_name, ' ', last_name) AS full_name
FROM employees;
```

### `SUBSTRING`
```sql
-- Extracts a substring from a string
SELECT SUBSTRING('Hello World', 7, 5) AS substring_value; -- Starts at position 7 and extracts 5 characters
```

### `LENGTH`
```sql
-- Returns the length of a string
SELECT LENGTH('Hello World') AS string_length;
```

### `TRIM`
```sql
-- Removes leading and trailing spaces from a string
SELECT TRIM('   Hello World   ') AS trimmed_string;
```

### `REPLACE`
```sql
-- Replaces all occurrences of a substring within a string
SELECT REPLACE('Hello World', 'World', 'SQL') AS replaced_string;
```

### Wildcard Characters

| Character      | Description |
|----------------|-------------|
| `%`            | Represents zero or more characters in a string (used with `LIKE`). |
| `_`            | Represents a single character in a string (used with `LIKE`). |

### `%`
```sql
-- Represents zero or more characters in a string (used with LIKE)
SELECT * FROM products
WHERE product_name LIKE 'Apple%'; -- Finds all products starting with 'Apple'
```

### `_`
```sql
-- Represents a single character in a string (used with LIKE)
SELECT * FROM customers
WHERE phone_number LIKE '5551_3%'; -- Finds phone numbers starting with '5551' followed by any single character and then more characters
```

### Views

| Keyword                    | Description |
|----------------------------|-------------|
| `CREATE VIEW`              | Creates a new view. |
| `ALTER VIEW`               | Modifies an existing view. |
| `DROP VIEW`                | Deletes a view. |
| `CREATE OR REPLACE VIEW`   | Creates a new view or replaces an existing one. |
| `SELECT * FROM <view_name>`| Retrieves data from a view. |

### `CREATE VIEW`
```sql
-- Creates a new view
CREATE VIEW top_customers AS
SELECT customer_id, customer_name, SUM(order_total) AS total_spent
FROM orders
GROUP BY customer_id, customer_name
HAVING SUM(order_total) > 10000;
```

### `ALTER VIEW`
```sql
-- Modifies an existing view
ALTER VIEW top_customers
AS
SELECT customer_id, customer_name, SUM(order_total) AS total_spent
FROM orders
GROUP BY customer_id, customer_name
HAVING SUM(order_total) > 20000;
```

### `DROP VIEW`
```sql
-- Deletes a view
DROP VIEW IF EXISTS top_customers;
```

### `CREATE OR REPLACE VIEW`
```sql
-- Creates a new view or replaces an existing one
CREATE OR REPLACE VIEW top_products AS
SELECT product_id, product_name, AVG(product_price) AS average_price
FROM products
GROUP BY product_id, product_name;
```

### `SELECT * FROM <view_name>`
```sql
-- Retrieves data from a view
SELECT * FROM top_customers;
```

### PostgreSQL-Specific Keywords

| Keyword                    | Description                |
|----------------------------|----------------------------|
| `DO`                       | Executes an anonymous code block. |
| `ILIKE`                    | Case-insensitive version of `LIKE`. |
| `PERFORM`                  | Executes a function and discards the result. |
| `SERIAL`                   | Creates an auto-incrementing integer column. |
| `UNLISTEN`                 | Stops listening for a notification. |
| `VACUUM`                   | Reclaims storage and updates statistics for a table. |
| `RETURNING`                | Returns the values of columns after an `INSERT`, `UPDATE`, or `DELETE`. |
| `ARRAY`                    | Allows the use of array data types. |
| `ANY`                      | Tests whether a value matches any value in a subquery or list. |
| `ALL`                      | Tests whether a value matches all values in a subquery or list. |
| `pg_catalog`               | Schema that contains system views and data types. |
| `information_schema`       | Standard schema containing views that define the structure of the database. |
| `pg_views`                 | System view that provides information about views in the current database. |
| `pg_tables`                | System view that provides information about tables in the current database. |
| `pg_datatype`              | System view that provides information about data types in the current database.|

### `DO`
```sql
-- Executes an anonymous code block
DO $$
BEGIN
    RAISE NOTICE 'Hello, PostgreSQL!';
END $$;
```

### `ILIKE`
```sql
-- Case-insensitive version of LIKE
SELECT * FROM employees
WHERE first_name ILIKE 'jo%';
```

### `PERFORM`
```sql
-- Executes a function and discards the result
PERFORM expensive_operation();
```

### `SERIAL`
```sql
-- Creates an auto-incrementing integer column
CREATE TABLE users (
    user_id SERIAL PRIMARY KEY,
    username VARCHAR(50) NOT NULL,
    email VARCHAR(100) NOT NULL
);
```

### `UNLISTEN`
```sql
-- Stops listening for a notification
UNLISTEN my_channel;
```

### `VACUUM`
```sql
-- Reclaims storage and updates statistics for a table
VACUUM FULL VERBOSE ANALYZE orders;
```

### `RETURNING`
```sql
-- Returns the values of columns after an INSERT, UPDATE, or DELETE
INSERT INTO products (product_name, price)
VALUES ('New Product', 99.99)
RETURNING product_id, product_name, price;
```

### `ARRAY`
```sql
-- Allows the use of array data types
SELECT product_id, product_name, ARRAY['red', 'green', 'blue'] AS colors
FROM products;
```

### `ANY and ALL`
```sql
-- Tests whether a value matches any value or all values in a subquery or list
SELECT * FROM products
WHERE price > ANY (SELECT price FROM expensive_products);

SELECT * FROM products
WHERE price <= ALL (SELECT price FROM affordable_products);
```

### `pg_catalog`
```sql
-- Schema that contains system views and data types
SELECT * FROM pg_catalog.pg_tables;
```

### `information_schema`
```sql
-- Standard schema containing views that define the structure of the database
SELECT * FROM information_schema.tables
WHERE table_schema = 'public';
```

### `pg_views`
```sql
-- System view that provides information about views in the current database
SELECT * FROM pg_views;
```

### `pg_tables`
```sql
-- System view that provides information about tables in the current database
SELECT * FROM pg_tables;
```

### `pg_datatype`
```sql
-- System view that provides information about data types in the current database
SELECT * FROM pg_datatype;
```
