# mysql


SHOW DATABASES; -- show all databases;

USE dbname; -- SELECT THE DATABASE

SHOW TABLES; -- SHOW ALL TABLES IN SELECTED DATABASE

DESCRIBE tablename; -- Show structure of table

DROP TABLE tablename; -- Delete table

DROP DATABASE dbname; -- delete database


-- Crete table
CREATE TABLE tablename(
    column1 columnType extraOptions,
    column2 columnType,
)  

-- Create table
CREATE TABLE category(
	id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(255) NOT NULL,
    nam VARCHAR(255) NOT NULL
)


-- Alter commands

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
