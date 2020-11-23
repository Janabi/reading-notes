# SQL
## What is sql stand for?

Check this [link](https://sqlbolt.com/lesson/introduction) as a reference for these notes.

**SQL** is a ***Structured Query Language*** which allow you to create a user query, manipulate and transfer data from rational database. ***Rational Database*** means that a coollections of two-dimensional tables, where each tabls has a fixed number of column (that has a unique title) and a a changable number of rows where they represent the values of that columns.

### How to create a table from scratch?
```
CREATE TABLE IF NOT EXISTS mytable (
    column DataType TableConstraint DEFAULT default_value,
    another_column DataType TableConstraint DEFAULT default_value,
    …
);
```
The previous block of codes was aimed to create a new table by using a preserve word in sql **(CREATE TABLE)** but as you can see there is a sentence **(IF NOT EXIST)** to check weither that table is actually exist in your file or not been created yet.
Then, on the next line you will declare the title of the first column and its data type (Boolean, Varchar, Text, Integer, Double, Float,...). Also, you are free to apply table constraint values in each columns, so lets take a look at its most important and majorly used values and what does each value mean?

Value# | Description
----------|------------
Primary Key     |means that each value of this column should be unique for each row. 
Autoincrement     |this is especial for integer type column and it will increase by one for each row. 
unique     |means each single value of this column should be unique and differ than the rest of rows
Not Null     |that mean you don't have to leave the value of this column empty.

Therefore, definitely there are so much more but we only walk you through the most used ones. 

**In addition, you can alter your table by applying the following syntax:**
```
ALTER TABLE mytable
ADD column DataType OptionalTableConstraint 
    DEFAULT default_value;
```
The previous example meant to add a new column name something with a certain data type and to give this column a value for all existing rows.
Also, we can remove an entire column from the table by the following script:
```
ALTER TABLE mytable
DROP column_to_be_deleted;
```
To rename an existing table into another name;
```
ALTER TABLE mytable
RENAME TO new_table_name;
```

In addition, you can as well drop or remove the whole table by using the following syntax:
```
DROP TABLE IF EXISTS mytable;
```

### Selecting an existing table
To select a certain column from an existing table, we have to type the name of that column or if you would like more one column just used ','. However, to select the whole table just used asterisk'*'
```
SELECT column, another_column, …
FROM mytable;
```
```
SELECT * 
FROM mytable;
```

### Selecting Queries with constraints
if we have a lots of data (rows) for each columns and we only want a certain range of values. Then, sql has a query where you can select that with this following syntax:
```
SELECT column, another_column, …
FROM mytable
WHERE condition
    AND/OR another_condition
    AND/OR …;
```
Operator# | Description
----------|------------
=, !=, < <=, >, >=     |Standard numerical operators
BETWEEN … AND …     |Number is within range of two values (inclusive)
NOT BETWEEN … AND      |Number is not within range of two values (inclusive)
IN    |Number exists in a list
NOT IN  |Number does not exist in a list

Therefore, there are other operators for string data type which they apply for the same previous syntax but fist thing you have to read them carefully and then try to do that on your table.
Check these operators on the following links:
[string_operators](https://sqlbolt.com/lesson/select_queries_with_constraints_pt_2)

