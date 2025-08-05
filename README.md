# Employee Data Insertion and Management

## 📌 Objective
This mini-project demonstrates basic SQL operations — specifically `INSERT`, `UPDATE`, and `DELETE` — on an `employees` table using SQLite. It also covers handling `NULL` values and default data types.

## 🛠️ Tools Used
- SQLiteStudio
- DB Fiddle (SQLite)

## 📂 Files
- `employee_data.sql`: SQL script to create the table and perform data operations.
- `README.md`: This documentation file.

## 🧱 Table Structure

### Table: `employees`

| Column     | Type     | Description                   |
|------------|----------|-------------------------------|
| id         | INTEGER  | Primary Key                   |
| name       | TEXT     | Employee's name (NOT NULL)    |
| department | TEXT     | Department (e.g., HR, IT)     |
| salary     | REAL     | Monthly salary                |
| join_date  | DATE     | Date the employee joined      |

---

## ▶️ Sample Insert Statement

```sql
INSERT INTO employees (id, name, department, salary, join_date) VALUES (1, 'Prasad', 'HR', 50000.00, CURRENT_DATE());
insert into employees (id, name, department, salary, join_date)values (2, 'Raghu', 'MANAGER', 42000.00, CURRENT_DATE());
insert into employees (id, name, department, salary, join_date)values (3, 'Seetha', 'MANAGER', 45000.00, CURRENT_DATE());
insert into employees (id, name, department, salary, join_date)values (4, 'Lakshmi', 'IT', 55000.00, CURRENT_DATE());
insert into employees (id, name, department, salary, join_date)values (5, 'Ramu', 'MANAGER', 45000.00, CURRENT_DATE());

UPDATE employees SET department = 'Finance' WHERE id = 2;

DELETE FROM employees WHERE id = 5;
