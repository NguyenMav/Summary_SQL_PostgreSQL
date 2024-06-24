# PostgreSQL Basics Cheat Sheet
| **Category**                | **Keywords/Functions**                                           |
|-----------------------------|------------------------------------------------------------------|
| **Sample Data**             | `COUNTRY`, `CITY`                                               |
| **Querying Single Table**   | `SELECT`, `FROM`, `ORDER BY`, `ASC`, `DESC`, `WHERE`, `LIKE`, `BETWEEN`, `IS NOT NULL` |
| **Aliases**                 | `AS`                                                            |
| **Joins**                   | `INNER JOIN`, `LEFT JOIN`, `RIGHT JOIN`, `FULL JOIN`, `CROSS JOIN`, `NATURAL JOIN` |
| **Aggregation and Grouping**| `GROUP BY`, `COUNT`, `AVG`, `MAX`, `MIN`, `SUM`                 |
| **Subqueries**              | `IN`, `EXISTS`                                                  |
| **Set Operations**          | `UNION`, `UNION ALL`, `INTERSECT`, `EXCEPT`                     |
| **Text Functions**          | `CONCAT`, `LIKE`, `SUBSTRING`, `REPLACE`, `LOWER`, `UPPER`      |
| **Numeric Functions**       | `ROUND`, `CEIL`, `FLOOR`, `MOD`, `ABS`, `SQRT`                  |
| **Null Handling**           | `IS NULL`, `IS NOT NULL`, `COALESCE`, `NULLIF`                  |
| **Case**                    | `CASE`, `WHEN`, `THEN`, `ELSE`                                  |
| **Other Operators**         | `AND`, `OR`, `NOT`, `<>`, `!=`, `>`, `<`, `>=`, `<=`            |
| **Basic Math Operations**   | `+`, `-`, `*`, `/`, `%`                                         |
| **Data Types and Casting**  | `CAST`, `DOUBLE PRECISION`                                      |
| **Miscellaneous**           | `HAVING`                                                        |
| **Example Queries**         | `SELECT COUNT(*)`, `SELECT DISTINCT`                            |
| **Troubleshooting**         | `NULL`, `NULLIF`                                                |


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

- [Data Query Language (DQL) Keywords](#data-query-language-dql-keywords)
- [Data Manipulation Language (DML) Keywords](#data-manipulation-language-dml-keywords)
- [Data Definition Language (DDL) Keywords](#data-definition-language-ddl-keywords)
- [Data Control Language (DCL) Keywords](#data-control-language-dcl-keywords)
- [Transaction Control Language (TCL) Keywords](#transaction-control-language-tcl-keywords)
- [JOIN Keywords](#join-keywords)
- [Aggregation Functions](#aggregation-functions)
- [Ranking Functions](#ranking-functions)
- [Window Functions](#window-functions)
- [Numeric Functions](#numeric-functions)
- [Null Handling Functions](#null-handling-functions)
- [String Functions](#string-functions)
- [Wildcard Characters](#wildcard-characters)
- [Views](#views)
- [PostgreSQL-Specific Keywords](#postgresql-specific-keywords)

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

### Data Control Language (DCL) Keywords

| Keyword       | Description |
|---------------|-------------|
| `GRANT`       | Gives user permissions. |
| `REVOKE`      | Removes user permissions. |

### Transaction Control Language (TCL) Keywords

| Keyword           | Description |
|-------------------|-------------|
| `COMMIT`          | Saves all changes made in the current transaction. |
| `ROLLBACK`        | Reverts all changes made in the current transaction. |
| `SAVEPOINT`       | Sets a point within a transaction to which a rollback can occur. |
| `SET TRANSACTION` | Sets transaction properties. |

### JOIN Keywords

| Keyword       | Description |
|---------------|-------------|
| `INNER JOIN`  | Returns records with matching values in both tables. |
| `LEFT JOIN`   | Returns all records from the left table and matched records from the right table. |
| `RIGHT JOIN`  | Returns all records from the right table and matched records from the left table. |
| `FULL JOIN`   | Returns all records when there is a match in either left or right table. |
| `CROSS JOIN`  | Returns the Cartesian product of both tables. |
| `SELF JOIN`   | Joins a table with itself. |

### Aggregation Functions

| Function       | Description |
|----------------|-------------|
| `COUNT`        | Returns the number of rows that match a specified condition. |
| `SUM`          | Returns the total sum of a numeric column. |
| `AVG`          | Returns the average value of a numeric column. |
| `MIN`          | Returns the smallest value of a column. |
| `MAX`          | Returns the largest value of a column. |

### Ranking Functions

| Function       | Description |
|----------------|-------------|
| `ROW_NUMBER`   | Assigns a unique number to each row according to the order specified. |
| `RANK`         | Assigns a rank to each row within the partition of a result set. |
| `DENSE_RANK`   | Similar to `RANK` but does not leave gaps in the ranking sequence. |
| `NTILE`        | Divides the result set into a specified number of roughly equal parts. |

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

### Null Handling Functions

| Function       | Description |
|----------------|-------------|
| `COALESCE`     | Returns the first non-null value in a list. |
| `NULLIF`       | Returns null if the two arguments are equal. |
| `IS NULL`      | Checks if a value is null. |
| `IS NOT NULL`  | Checks if a value is not null. |

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

### Wildcard Characters

| Character      | Description |
|----------------|-------------|
| `%`            | Represents zero or more characters in a string (used with `LIKE`). |
| `_`            | Represents a single character in a string (used with `LIKE`). |

### Views

| Keyword                    | Description |
|----------------------------|-------------|
| `CREATE VIEW`              | Creates a new view. |
| `ALTER VIEW`               | Modifies an existing view. |
| `DROP VIEW`                | Deletes a view. |
| `CREATE OR REPLACE VIEW`   | Creates a new view or replaces an existing one. |
| `SELECT * FROM <view_name>`| Retrieves data from a view. |

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

