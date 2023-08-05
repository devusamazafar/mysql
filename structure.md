# MYSQL structure commands
## show all tables

```

SHOW DATABASES; -- show all databases;

```

## select a database

```
 USE dbname; -- SELECT THE DATABASE 
```


## show all tables in selected database

```
 SHOW TABLES; -- SHOW ALL TABLES IN SELECTED DATABASE 
```


## show structure of table

```
 DESCRIBE tablename; -- Show structure of table 
```


## delete a table

```
 DROP TABLE tablename; -- Delete table 
```


## delete a database

```
 DROP DATABASE dbname; -- delete database 
```



## delete a database

## show  query for existing table
```
SHOW CREATE TABLE `user`
```

## Create table



```

-- Crete table
CREATE TABLE tablename(
    column1 columnType extraOptions,
    column2 columnType,
)  

```


### create category table 

```

-- Create table
CREATE TABLE category(
	id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(255) NOT NULL,
    nam VARCHAR(255) NOT NULL
)

```

### create category user 

```

CREATE TABLE `user`(
    id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(255) NOT NULL
    dob2 TIMESTAMP NOT NULL DEFAULT CURRENT_TIMESTAMP ,
    gender ENUM('male', 'female', 'email', 'gmail') NOT NULL,
    name2 VARCHAR(255) DEFAULT "OSMAMA",
);

```



-- Alter commands

```

ALTER TABLE tablename command;

ALTER TABLE category DROP nam; -- Delete nam field from category table

-- Add new column
ALTER TABLE category ADD parent INT NOT NULL DEFAULT '0' AFTER `name`;

-- Rename table
RENAME TABLE old_name TO new_name;
-- or
ALTER TABLE old_name RENAME TO new_name; 
-- or
ALTER TABLE old_name RENAME new_name;  

```
