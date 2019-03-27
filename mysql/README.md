### MYSQL 

1. Login 
```mysql
  mysql -u user -p
  # If not running on local host
  mysql -u user -p -h hostName
```  
2. Create Database
```mysql
  CREATE DATABASE database_name;
```
3. Show Databases
```mysql
  SHOW DATABASES;
  SHOW {DATABASES | SCHEMAS}
    [LIKE 'pattern' | WHERE expr]

```
4. Show Tables
```mysql
  SHOW TABLES;
  SHOW [FULL] TABLES [{FROM | IN} db_name]
    [LIKE 'pattern' | WHERE expr]
```    
5. Grant
```mysql
  GRANT ALL PRIVILEGES ON database_name.* TO 'user'@'host_name' IDENTIFIED BY 'password';
```

