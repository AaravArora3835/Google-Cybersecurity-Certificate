# **2025-12-05_SQL_Intermediate_Lab.md**

## SQL Intermediate Lab — UPDATE, INSERT, DELETE, ORDER BY

---

## Overview

This lab provided hands-on practice with intermediate SQL operations using a real MariaDB/MySQL database inside a Linux virtual machine. The goal was to create a small dataset and then modify it using `INSERT`, `UPDATE`, and `DELETE`, as well as sort the results using `ORDER BY`. These operations support the concepts from Course 4 Module 4 and prepare for future SQL injection work in VulnForge.

---

## Lab Environment

* OS: Kali Linux (VirtualBox)
* Database: MariaDB (MySQL-compatible)
* Database name: `training`
* Table name: `employees`
* Access method: `sudo mysql` interactive shell

---

## Step 1: Start MariaDB and Enter SQL Shell

Commands:

```bash
sudo systemctl start mariadb
sudo mysql
```

Notes:

* `systemctl` started the MariaDB service.
* `sudo mysql` opened the SQL shell as root, allowing database and table management.

---

## Step 2: Create Database and Table

Commands:

```sql
CREATE DATABASE training;
USE training;

CREATE TABLE employees (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(50),
    role VARCHAR(50),
    salary INT
);
```

Notes:

* `training` was created as the lab database.
* The `employees` table includes an auto-incrementing primary key and fields for name, role, and salary.
* This table structure is simple but realistic enough for practicing data modification.

---

## Step 3: Insert Initial Records

Commands:

```sql
INSERT INTO employees (name, role, salary)
VALUES
('Aarav', 'Intern', 45000),
('Maya', 'Analyst', 60000),
('Jordan', 'Manager', 85000),
('Sasha', 'Director', 120000);
```

Verification:

```sql
SELECT * FROM employees;
```

Notes:

* Four employees were inserted with different roles and salary levels.
* The `SELECT` query confirmed that all rows were stored correctly and that the `id` values auto-incremented as expected.

---

## Step 4: Update Existing Records

Commands:

```sql
UPDATE employees
SET salary = 65000
WHERE role = 'Analyst';

UPDATE employees
SET role = 'Senior Intern'
WHERE name = 'Aarav';
```

Verification:

```sql
SELECT * FROM employees;
```

Notes:

* The salary for the `Analyst` role was increased to 65,000.
* The role for `Aarav` was changed from `Intern` to `Senior Intern`.
* The verification query confirmed that only the intended rows were modified.

---

## Step 5: Delete a Record

Commands:

```sql
DELETE FROM employees
WHERE name = 'Jordan';
```

Verification:

```sql
SELECT * FROM employees;
```

Notes:

* The row for `Jordan` was removed from the table.
* The `DELETE` statement permanently removed the record, demonstrating the impact of destructive commands.
* Verification ensured there were no unintended deletions.

---

## Step 6: Sort Data Using ORDER BY

Commands:

```sql
SELECT * FROM employees
ORDER BY salary DESC;
```

Notes:

* Sorting by salary in descending order showed the highest earning roles first.
* This type of query is useful for identifying outliers, high-value targets, or unusual patterns in a dataset.

---

## Step 7: Final Output and Evidence

Final query for screenshot:

```sql
SELECT * FROM employees ORDER BY salary DESC;
```

Evidence:

* Screenshot captured of the final sorted `employees` table:

  * `2025-12-05_SQL_IntermediateLab_Completed.png`

This screenshot shows the table after all inserts, updates, deletions, and sorting operations were completed.

---

## Reflection

This lab improved my understanding of how SQL can modify data stored in a relational database. Creating a table and then using `INSERT` made it clear how structured records are added to a system. Using `UPDATE` and `DELETE` showed how powerful and potentially risky modification commands can be if they are not carefully scoped with `WHERE` conditions. The `ORDER BY` clause demonstrated how sorting results can help analysts quickly identify the most important entries, such as highest salaries or critical records. These skills directly connect to SQL injection concepts, because attackers often try to manipulate the same operations in unintended ways. Overall, this lab made SQL feel more practical and highlighted the importance of precision and verification when running database commands.
