# SQL cheatsheet by Aman

Windows admin part:
SELECT NAME 

PHYSICAL SCHEMA: which is created by company like logs
LOGICAL SCHEMA: which is created by us 

## To show the name of databases created in the SQL server
SELECT NAME FROM sys.databases

## To create the database
CREATE DATABASE db_name

## To create the table in the database
CREATE TABLE_NAME (
    FIELD_NAME DATA_TYPE IDENTITY(STARTING FROM, INCREASE BY) PRIMARY KEY,
)
