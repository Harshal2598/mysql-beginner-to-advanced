🏆 Top 20 Most Important SQL Queries (With Examples & Effects)
These 20 commands are the most commonly used in real development, interviews, and daily SQL work.

---
```sql
## 1. SELECT  
Retrieves data from a table.


SELECT * FROM employees;
Effect: Shows all rows and columns from employees.

2. SELECT (specific columns)
sql
Copy code
SELECT name, salary FROM employees;
Effect: Returns only selected columns.

3. WHERE (filter data)
sql
Copy code
SELECT * FROM employees WHERE salary > 50000;
Effect: Fetches only employees earning above 50k.

4. INSERT
sql
Copy code
INSERT INTO employees (name, salary) VALUES ('Harshal', 45000);
Effect: Adds a new row into the table.

5. UPDATE
sql
Copy code
UPDATE employees SET salary = 60000 WHERE id = 3;
Effect: Updates salary of employee with id = 3.

6. DELETE
sql
Copy code
DELETE FROM employees WHERE id = 5;
Effect: Removes the row where id = 5.

7. ORDER BY
sql
Copy code
SELECT * FROM employees ORDER BY salary DESC;
Effect: Sorts employees by highest salary first.

8. LIMIT
sql
Copy code
SELECT * FROM employees LIMIT 5;
Effect: Shows only the first 5 rows.

9. DISTINCT
sql
Copy code
SELECT DISTINCT department FROM employees;
Effect: Removes duplicates; shows unique departments.

10. COUNT()
sql
Copy code
SELECT COUNT(*) FROM employees;
Effect: Returns total number of rows.

11. SUM()
sql
Copy code
SELECT SUM(salary) FROM employees;
Effect: Gives total salary paid to employees.

12. AVG()
sql
Copy code
SELECT AVG(salary) FROM employees;
Effect: Shows average salary.

13. GROUP BY
sql
Copy code
SELECT department, COUNT(*) 
FROM employees 
GROUP BY department;
Effect: Shows number of employees per department.

14. HAVING (filter groups)
sql
Copy code
SELECT department, COUNT(*) 
FROM employees 
GROUP BY department
HAVING COUNT(*) > 5;
Effect: Shows departments with more than 5 employees.

15. INNER JOIN
sql
Copy code
SELECT e.name, d.department_name
FROM employees e
INNER JOIN departments d
ON e.dept_id = d.id;
Effect: Combines matching rows from both tables.

16. LEFT JOIN
sql
Copy code
SELECT e.name, d.department_name
FROM employees e
LEFT JOIN departments d
ON e.dept_id = d.id;
Effect: Shows all employees, including those without a department match.

17. CREATE TABLE
sql
Copy code
CREATE TABLE employees (
  id INT PRIMARY KEY,
  name VARCHAR(100),
  salary DECIMAL(10,2)
);
Effect: Creates a new table.

18. ALTER TABLE (Add column)
sql
Copy code
ALTER TABLE employees ADD age INT;
Effect: Adds a new column to the table.

19. DROP TABLE
sql
Copy code
DROP TABLE employees;
Effect: Deletes the table and its data permanently.

20. SUBQUERY
sql
Copy code
SELECT name 
FROM employees 
WHERE salary > (SELECT AVG(salary) FROM employees);
Effect: Shows employees earning above the average salary.
