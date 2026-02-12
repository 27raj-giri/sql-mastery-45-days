# 📅 Day 1 – SELECT Basics

## 🎯 Objective
Build a strong foundation in SQL by learning how to retrieve data using SELECT queries.

---

# 🧠 Concepts Covered

## 1. What is SQL?
SQL (Structured Query Language) is used to interact with relational databases.

It allows you to:
- Retrieve data
- Insert data
- Update data
- Delete data

---

## 2. SELECT Statement

### Basic Syntax
```sql
SELECT column_name
FROM table_name;

Select All Columns
SELECT * FROM students;

3. Selecting Specific Columns
SELECT name, age FROM students;

4. WHERE Clause (Filtering Data)

Used to filter rows based on conditions.

SELECT * FROM students
WHERE age = 21;

Comparison Operators
Operator	Meaning
=	Equal
!=	Not Equal
>	Greater than
<	Less than
>=	Greater than equal
<=	Less than equal
5. Logical Operators
Operator	Meaning
AND	Both conditions must be true
OR	At least one condition true
NOT	Reverse condition
Example
SELECT * FROM students
WHERE grade = 'A' AND marks > 85;

6. BETWEEN
SELECT * FROM students
WHERE age BETWEEN 20 AND 22;

7. IN Operator
SELECT * FROM students
WHERE city IN ('Delhi', 'Mumbai', 'Pune');

8. LIKE (Pattern Matching)
Pattern	Meaning
'A%'	Starts with A
'%a'	Ends with a
'%or%'	Contains "or"
SELECT * FROM students
WHERE name LIKE 'A%';

9. ORDER BY (Sorting)
Ascending
SELECT * FROM students ORDER BY age ASC;

Descending
SELECT * FROM students ORDER BY marks DESC;

10. LIMIT & OFFSET
Top N rows
SELECT * FROM students
ORDER BY marks DESC
LIMIT 3;

Pagination
SELECT * FROM students
ORDER BY marks DESC
LIMIT 3 OFFSET 1;

📊 Dataset Used

Table: students

Columns:

id

name

age

grade

city

marks

📈 Key Learnings

SELECT is the foundation of SQL

WHERE filters rows

ORDER BY sorts data

LIKE helps in pattern searching

LIMIT helps in top-N analysis

🌍 Real World Use Cases

User filtering in applications

Customer segmentation

Top performer analysis

Dashboard queries

Data cleaning

🏁 Summary

Day 1 focused on core SQL retrieval concepts.

These basics are essential for:

Data Analytics

Backend systems

Product analytics

Business intelligence

🔜 Next Step

➡️ Day 2 – WHERE Conditions Deep Dive
