# SQL Commands Cheatsheet


### Data Definition Language 
[deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database]

* CREATE [used to create the database or its objects (like table, index, function, views, store procedure and triggers)]

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


* ALTER [used to alter the structure of the database]

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


* TRUNCATE [used to remove all records from a table, including all spaces allocated for the records are removed]


[Remove all the records from a table.](#)
```sql
TRUNCATE TABLE table_name
```



* DROP [used to delete objects from the database]


[Remove a table from the database.](#)
```sql
DROP TABLE table_name;
```
[Delete the complete database](#)
```sql
DROP DATABASE database_name;
```



* RENAME [used to rename an object existing in the database]


[Set a new name for any existing table](#)
```sql
RENAME TABLE old_table_name to new_table_name;
```


* COMMENT [used to add comments to the data dictionary]


---

### Data Query Language 
[used for performing queries on the data within schema objects] 

* SELECT [used to retrieve data from the database]


### Data Manipulation Language
[deals with the manipulation of data present in the database]

* INSERT [used to insert data into a table]

* UPDATE [used to update existing data within a table]

* DELETE [used to delete records from a database table]

* MERGE [can handle inserts, updates, and deletes all in a single transaction without having to write separate logic for each of these]

* CALL [to execute a routine (a standalone procedure or function, or a procedure or function defined within a type or package)]

* EXPLAIN PLAN [displays execution plans chosen by the optimizer for SELECT , UPDATE , INSERT , and DELETE statements]

* LOCK TABLE [to lock one or more tables, table partitions, or table subpartitions in a specified mode.]


### Data Control Language
[deal with the rights, permissions and other controls of the database system.]


* GRANT [gives users access privileges to the database]
* REVOKE [withdraw user’s access privileges given by using the GRANT command.]


### Transaction Control Language
[deal with the transaction within the database.]

* COMMIT [commits a Transaction.]

* ROLLBACK [rollbacks a transaction in case of any error occurs.]

* SAVEPOINT [sets a savepoint within a transaction.]

* SET TRANSACTION [specify characteristics for the transaction.]
