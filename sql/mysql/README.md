1. Create Database
```mysql
  CREATE DATABASE database_name;
```
2. Show Databases
```mysql
  SHOW DATABASES;
  SHOW {DATABASES | SCHEMAS}
    [LIKE 'pattern' | WHERE expr]

```
3. Show Tables
```mysql
  SHOW TABLES;
  SHOW [FULL] TABLES [{FROM | IN} db_name]
    [LIKE 'pattern' | WHERE expr]
```    
4. Grant
```mysql
  GRANT ALL PRIVILEGES ON database_name.* TO 'user'@'host_name' IDENTIFIED BY 'password';
```

