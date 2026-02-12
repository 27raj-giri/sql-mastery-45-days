# Day 1 – SELECT Basics

## Objective
Build a strong foundation in SQL by learning how to retrieve data using SELECT queries.

--------------------------------------------------

WHAT IS SQL

SQL (Structured Query Language) is used to interact with relational databases.

It allows you to:
- Retrieve data
- Insert data
- Update data
- Delete data

--------------------------------------------------

SELECT STATEMENT

Basic Syntax:

SELECT column_name
FROM table_name;

Example:

SELECT * FROM students;

--------------------------------------------------

SELECT SPECIFIC COLUMNS

SELECT name, age FROM students;

--------------------------------------------------

WHERE CLAUSE (FILTERING DATA)

Used to filter rows based on conditions.

Example:

SELECT * FROM students
WHERE age = 21;

Common Operators:
=   Equal
!=  Not equal
>   Greater than
<   Less than
>=  Greater than equal
<=  Less than equal

--------------------------------------------------

LOGICAL OPERATORS

AND  -> both conditions must be true
OR   -> at least one condition true
NOT  -> reverse condition

Example:

SELECT * FROM students
WHERE grade = 'A' AND marks > 85;

--------------------------------------------------

BETWEEN

SELECT * FROM students
WHERE age BETWEEN 20 AND 22;

--------------------------------------------------

IN OPERATOR

SELECT * FROM students
WHERE city IN ('Delhi', 'Mumbai', 'Pune');

--------------------------------------------------

LIKE (PATTERN MATCHING)

'A%'   -> starts with A
'%a'   -> ends with a
'%or%' -> contains "or"

Example:

SELECT * FROM students
WHERE name LIKE 'A%';

--------------------------------------------------

ORDER BY (SORTING)

Ascending:

SELECT * FROM students
ORDER BY age ASC;

Descending:

SELECT * FROM students
ORDER BY marks DESC;

--------------------------------------------------

LIMIT & OFFSET

Top N rows:

SELECT * FROM students
ORDER BY marks DESC
LIMIT 3;

Pagination (skip rows):

SELECT * FROM students
ORDER BY marks DESC
LIMIT 3 OFFSET 1;

--------------------------------------------------

DATASET USED

Table: students

Columns:
id
name
age
grade
city
marks

--------------------------------------------------

KEY LEARNINGS

- SELECT is the foundation of SQL
- WHERE filters rows
- ORDER BY sorts data
- LIKE helps in pattern searching
- LIMIT helps in top N analysis

--------------------------------------------------

REAL WORLD USE CASES

- User filtering in applications
- Customer segmentation
- Top performer analysis
- Dashboard queries
- Data cleaning

--------------------------------------------------

SUMMARY

Day 1 focused on core SQL retrieval concepts.

These basics are essential for:
- Data Analytics
- Backend systems
- Product analytics
- Business intelligence

--------------------------------------------------

NEXT STEP

Day 2 – WHERE Conditions Deep Dive
