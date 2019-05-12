### Basic ansi CRUD operations

#### Read
```sql
SELECT column1, column2, ...
FROM table_name
WHERE some_condition;

SELECT * 
FROM table_name
WHERE some_condition;

-- Distinct works on a single column
SELECT DISTINCT column
FROM table_name; 
```
#### Add
```sql
INSERT INTO table_name (column1, column2, column3, ...)
VALUES (value1, value2, value3, ...); 

-- Inserting all of the values
INSERT INTO table_name
VALUES (value1, value2, value3, ...); 
```

#### Update
```sql
UPDATE table_name
SET column1 = value1, column2 = value2, ...
WHERE condition;
```

#### Delete
```sql
DELETE FROM table_name WHERE condition;
```

#### Inner Join
```sql
SELECT column_name(s)
FROM table1
INNER JOIN table2
ON table1.column_name = table2.column_name;
```
