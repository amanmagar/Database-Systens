# SQL cheatsheet by Aman

Windows admin part:
SELECT NAME 

PHYSICAL SCHEMA: which is created by company like logs <br>
LOGICAL SCHEMA: which is created by us 

## To show the name of databases created in the SQL server
SELECT NAME FROM sys.databases

## To create the database
CREATE DATABASE db_name

## To create the table in the database
CREATE TABLE_NAME (
    FIELD_NAME DATA_TYPE IDENTITY(STARTING FROM, INCREASE BY) PRIMARY KEY,
)

## To add foreign key to the table
CREATE TABLE_NAME (
    FIELD_NAME DATA_TYPE IDENTITY(STARTING FROM, INCREASE BY) PRIMARY KEY,
    FIELD_NAME DATA_TYPE FOREIGN KEY REFERENCES TABLE_NAME(PRIMARY KEY_FIELD),
)

## To insert the data into the database
INSERT INTO tablename (col1, col2) values (column1data, column2data )

## To update the data into the database
UPDATE INTO tablename SET (UpdData) where Col = value

## To delete the data from the database
DELETE FROM tablename where col = value;

## To add new column to the existing table
ALTER TABLE tablename ADD colname data type

## To delete the column of the exisitng table 
ALTER TABLE tablename DROP colname  

## To modify the datatype of the column of the existing table
ALTER TABLE tablename ALTER column colname datatype
