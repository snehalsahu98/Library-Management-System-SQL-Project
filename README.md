

# **Library Management System – SQL Project**

## **Table of Contents**

* Project Overview
* Data Source
* Tools
* Data Preparation
* SQL Analysis
* Results
* Recommendations
* Limitations
* References

---

### **Project Overview**

The purpose of this project is to design and analyze a **Library Management System** using SQL.
The system manages books, members, employees, and branches to handle operations such as book issuance, returns, and performance reporting.
The objective is to build a structured relational database that supports efficient management of library operations and provides insights into book circulation, employee activity, and branch performance.

---

### **Data Source**

* **SQL Database:** Data is stored in related tables including books, members, employees, branch, issued_status, and return_status.
* **Sample Data:** Records were manually created to simulate real-world library transactions for testing and analysis.

---

### **Tools**

* **PostgreSQL / SQL Server:** Used for database design, querying, and data analysis.
* **PL/pgSQL:** Implemented to create stored procedures for automating book issue and return processes.
* **SQL DDL & DML:** Used for schema creation, data insertion, and CRUD operations.

---

### **Data Preparation**

* **Schema Creation:** Designed normalized tables with primary and foreign keys to ensure data integrity.
* **Data Type Formatting:** Ensured correct data types for numeric, text, and date fields.
* **Referential Integrity:** Defined foreign key constraints between all related tables.
* **Data Validation:** Checked for null values, duplicates, and ensured consistent data formatting.

---

### **SQL Analysis**

Key areas of analysis included:

* **Issued Books:** Identified books most frequently issued.
* **Overdue Books:** Detected books overdue beyond the 30-day return period.
* **Branch Performance:** Evaluated branches based on issues, returns, and rental income.
* **Employee Productivity:** Ranked employees by number of books issued.
* **Category Insights:** Calculated total rental income by book category.
* **Active Members:** Listed members who issued books recently.

Stored procedures were created for automation:

* `issue_book()`: Issues a book if available and updates its status to “no”.
* `add_return_records()`: Records book returns and updates the book’s status to “yes”.

---

### **Results**

* The database successfully models all key library operations, including book issuance and returns.
* Generated reports provided insights into branch and employee performance.
* Automated processes improved accuracy and reduced manual intervention.
* Identified high-demand and unreturned books to support better inventory decisions.

---

### **Recommendations**

* Implement a fine calculation system for overdue books.
* Integrate a reporting dashboard for real-time performance tracking.
* Automate notifications for members about due and overdue books.
* Use indexing and query optimization techniques for large datasets.

---

### **Limitations**

* Static dataset; does not support real-time data updates.
* Limited sample data for scalability testing.
* Does not currently track damaged or lost books.
* Minimal input validation and no user interface integration.

---

### **References**

* PostgreSQL Documentation – SQL Commands and Stored Procedures.
* SQL Server Developer Guide – Data Modeling and Query Optimization.
* Database Design Standards – Normalization and Referential Integrity.

---
