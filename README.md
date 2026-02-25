# 🏛️ Parks and Recreation: Database Schema & Management

## 📖 Table of Contents
* [Project Overview](#-project-overview)
* [Technical Skills Demonstrated](#-technical-skills-demonstrated)
* [Database Architecture](#-database-architecture)
* [Entity Relationship Logic](#-entity-relationship-logic)
* [Data Preview](#-data-preview)
* [How to Use](#-how-to-use)

---

## 📌 Project Overview
This project demonstrates the creation and management of a relational database system for the **Pawnee Parks and Recreation Department**. The goal was to design a structured environment to manage employee demographics, department details, and payroll data, ensuring data integrity and relational mapping between different organizational units.

---

## 🚀 Technical Skills Demonstrated
* **Database Design:** Implementing Primary Keys and managing table relationships.
* **SQL DDL (Data Definition Language):** Creating and structuring databases and tables using `CREATE`, `DROP`, and `USE`.
* **SQL DML (Data Manipulation Language):** Populating datasets using `INSERT INTO` statements.
* **Data Types & Constraints:** Using appropriate data types (`INT`, `VARCHAR`, `DATE`) and constraints (`NOT NULL`, `AUTO_INCREMENT`).

---

## 🏗️ Database Architecture
The database consists of three primary tables designed to be joined for comprehensive reporting:



| Table Name | Description | Key Columns |
| :--- | :--- | :--- |
| **`employee_demographics`** | Personal information (age, gender, birth date). | `employee_id` (PK) |
| **`employee_salary`** | Professional data (occupation, salary, dept link). | `employee_id`, `dept_id` |
| **`parks_departments`** | Department lookup table. | `department_id` (PK) |

### 🔗 Entity Relationship Logic
1. **Employee Link:** The `employee_id` serves as the unique identifier linking demographics to salary data.
2. **Department Link:** The `dept_id` in the salary table links to the `department_id` in the departments table, allowing for granular departmental analysis.

---

## 🖼️ Data Preview

### 1. Employee Demographics Table
*Contains personal identifiable information for the department staff.*
![Demographics Table](INSERT_DEMOGRAPHICS_IMAGE_NAME.png)

### 2. Employee Salary Table
*Tracks roles, compensation, and departmental assignments.*
![Salary Table](INSERT_SALARY_IMAGE_NAME.png)

### 3. Parks Departments Table
*The lookup table for all official Pawnee departments.*
![Departments Table](INSERT_DEPARTMENTS_IMAGE_NAME.png)

---

## 🛠️ How to Use
1. Ensure you have **MySQL Workbench** or any SQL client installed.
2. Clone this repository.
3. Run the `parks_and_recreation_setup.sql` script to generate the database and populate it with the sample data provided.

---

## 📈 Future Analysis Goals
With this foundation, the next steps include:
* **JOIN Operations:** Analyzing average salary per department.
* **Demographic Trends:** Calculating age distribution using `birth_date`.
* **Financial Insights:** Identifying top-earning roles within the Parks department vs. Finance.
* 
