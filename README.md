# SQL Commands Cheatsheet

## DDL [Data Manipulation Language]

* CREATE

[Creating a Database](#)
```sql 
CREATE DATABASE <DB_NAME>; 
```

[Creating a Table](#)
```sql
CREATE TABLE <TABLE_NAME>
(
    column_name1 datatype1,
    column_name2 datatype2,
    column_name3 datatype3,
    column_name4 datatype4
);
```


* ALTER

[Add a new Column](#)
```sql
ALTER TABLE table_name ADD(
    column_name datatype);
```
[Add multiple new Columns](#)
```sql
ALTER TABLE table_name ADD(
    column_name1 datatype1, 
    column-name2 datatype2, 
    column-name3 datatype3);
```
[Add Column with default value](#)
```sql
ALTER TABLE table_name ADD(
    column-name1 datatype1 DEFAULT some_value
);
```
[Modify an existing Column](#)
```sql
ALTER TABLE table_name modify(
    column_name datatype
);
```
[Rename a Column](#)
```sql
ALTER TABLE table_name RENAME 
    old_column_name TO new_column_name;
```
[Drop a column](#)
```sql
ALTER TABLE table_name DROP(
    column_name);
```


* TRUNCATE


[Remove all the records from a table.](#)
```sql
TRUNCATE TABLE table_name
```



* DROP


[Remove a table from the database.](#)
```sql
DROP TABLE table_name;
```
[Delete the complete database](#)
```sql
DROP DATABASE database_name;
```



* RENAME


[Set a new name for any existing table](#)
```sql
RENAME TABLE old_table_name to new_table_name;
```
