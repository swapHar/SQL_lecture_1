# SQL_lecture_1
# Basic SQL Syntax

Basic SQL cheatsheet for Jensen Education.

## Read/Select data

Read all columns and rows from a table

```SQL
SELECT * FROM table_name;
```

Pick specific columns to show

```SQL
SELECT column_1, column_2 FROM table_name;
```

Using WHERE to pick only certain rows

```SQL
SELECT * FROM table_name WHERE column_name = "some value";
```

## Insert, create data

Insert into all columns

```SQL
INSERT INTO table_name VALUES("1", "2", "3");
```

Insert into specific columns

```SQL
INSERT INTO table_name (column_1, column_2) VALUES ("1", "2");
```

Note: If the ID column has `AUTOINCREMENT` applied we do not use a value there. We can either use `NULL` or leave it out when inserting values.

## Change data

```SQL
UPDATE table_name SET column_to_change = "new value" WHERE column_name = "some value to search for";
```

Quick example:

```SQL
UPDATE bands SET band_name = "Metallica" where id = 3;
```

## Remove data

```SQL
DELETE FROM table_name WHERE column_name = "some value";
```

## Sort data

Sort by data in column

```SQL
SELECT * FROM table_name ORDER BY column_name;
```

Sort descending order

```SQL
SELECT * FROM table_name ORDER BY column_name DESC
```

Limit request to X results

```SQL
SELECT * FROM table_name LIMIT 3;
```

## Comments

```SQL
SELECT * FROM table_name --this is a comment
```
