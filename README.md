Parks and Recreation Department: Database Schema & Management
Project Overview
This project demonstrates the creation and management of a relational database system for the Pawnee Parks and Recreation Department. The goal was to design a structured environment to manage employee demographics, department details, and payroll data, ensuring data integrity and relational mapping between different organizational units.

Technical Skills Demonstrated
Database Design: Implementing Primary Keys and managing table relationships.

SQL DDL (Data Definition Language): Creating and structuring databases and tables using CREATE, DROP, and USE.

SQL DML (Data Manipulation Language): Populating datasets using INSERT INTO statements.

Data Types & Constraints: Using appropriate data types (INT, VARCHAR, DATE) and constraints (NOT NULL, AUTO_INCREMENT).

Database Architecture
The database consists of three primary tables designed to be joined for comprehensive reporting:

Entity Relationship logic
The Employee ID serves as the unique identifier linking demographics to salary data.

The Dept ID links employees to their respective department names in the lookup table, allowing for granular departmental analysis.

How to Use
Ensure you have MySQL Workbench or any SQL client installed.

Clone this repository.

Run the parks_and_recreation_setup.sql script to generate the database and populate it with the sample data provided.

Future Analysis Goals
With this foundation, the next steps for this project include:

Performing JOIN operations to analyze the average salary per department.

Calculating the age distribution of employees using birth_date.

Identifying top-earning roles within the Parks department vs. Finance.
