# DB201 - Module 1: Database Fundamentals

What is DBMS? Software to store and manage data. Eg: Oracle, MySQL.

**Why Oracle?** Used by banks, big companies in Ghana.

Key Terms:
- Table = Excel sheet
- Row = Record
- Column = Field

Oracle SQL - First Lab:
```sql
-- Create Database Table
CREATE TABLE Students (
  StudentID NUMBER PRIMARY KEY,
  FullName VARCHAR2(100),
  Department VARCHAR2(50)
);
INSERT INTO Students VALUES (1, 'Ama Mensah', 'IT');
SELECT * FROM Students;
COMMIT;

# Module 2: DDL & DML in Oracle

**DDL - Data Definition Language:**
```sql
-- Create, Alter, Drop
CREATE TABLE Lecturers (ID NUMBER, Name VARCHAR2(50));
ALTER TABLE Lecturers ADD Email VARCHAR2(100);
DROP TABLE Lecturers;

-- DML - Data Manipulation
INSERT INTO Students VALUES (2, 'Kwame', 'Accounting');
UPDATE Students SET Department='IT' WHERE StudentID=2;
DELETE FROM Students WHERE StudentID=2;

**FILE: `Database-Oracle/Module-03.md`**
```md

# Module 3: Advanced Queries & Joins

**SELECT with Conditions:**
```sql
SELECT FullName FROM Students WHERE Department='IT';
SELECT * FROM Students ORDER BY FullName ASC;

-- Joins - MOST IMPORTANT FOR EXAMS
SELECT S.FullName, C.CourseName
FROM Students S
JOIN Courses C ON S.CourseID = C.CourseID;

-- Functions
SELECT COUNT(*) AS TotalStudents FROM Students;
SELECT AVG(Age) FROM Students;

Assignment: Create 2 tables: Customers and Orders, then JOIN them.
