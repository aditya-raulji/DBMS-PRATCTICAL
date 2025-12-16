# 🗄️ DBMS Practical Project

<div align="center">

![Database](https://img.shields.io/badge/Database-SQL-blue)
![Status](https://img.shields.io/badge/Status-Complete-success)
![License](https://img.shields.io/badge/License-MIT-green)

**A comprehensive collection of SQL practical exercises covering database operations**

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Project Structure](#-project-structure)
- [Features](#-features)
- [Database Schema](#-database-schema)
- [Practical Questions](#-practical-questions)
- [Getting Started](#-getting-started)
- [SQL Operations Covered](#-sql-operations-covered)

---

## 🎯 Overview

This repository contains practical SQL exercises demonstrating fundamental database management operations. The project focuses on creating and manipulating a **Hotels** database table, covering essential SQL concepts including table creation, data insertion, updates, deletions, and aggregate functions.

```
┌─────────────────────────────────────────┐
│         DBMS PRACTICAL PROJECT          │
│                                         │
│  ┌──────────┐    ┌──────────┐         │
│  │   Q1.md  │───▶│   Q2.md  │         │
│  │  CREATE  │    │  DML &   │         │
│  │  TABLE   │    │  QUERIES │         │
│  └──────────┘    └──────────┘         │
│         │              │                │
│         └──────┬───────┘                │
│                ▼                        │
│         ┌──────────┐                    │
│         │  Hotels  │                    │
│         │  Table   │                    │
│         └──────────┘                    │
└─────────────────────────────────────────┘
```

---

## 📁 Project Structure

```
DBMS-PRATCTICAL/
│
├── README.md          # Project documentation
├── Q1.md              # Question 1: Table Creation
└── Q2.md              # Question 2: DML Operations
```

---

## ✨ Features

- ✅ **Table Creation** with constraints (Primary Key, Unique, NOT NULL)
- ✅ **Data Manipulation** (INSERT, UPDATE, DELETE)
- ✅ **Aggregate Functions** (SUM, AVG)
- ✅ **Proper SQL Syntax** and best practices
- ✅ **Well-documented** code with comments

---

## 🗃️ Database Schema

### Hotels Table

| Column Name       | Data Type    | Constraints                    |
|-------------------|--------------|--------------------------------|
| `hotel_id`        | INT          | PRIMARY KEY                    |
| `hotel_name`      | VARCHAR(60)  | UNIQUE                         |
| `city`            | VARCHAR(40)  | -                              |
| `rooms_available` | INT          | NOT NULL                       |

```
┌─────────────────────────────────────────────┐
│              Hotels Table                    │
├──────────┬──────────────┬────────┬──────────┤
│ hotel_id │ hotel_name   │ city   │ rooms_...│
├──────────┼──────────────┼────────┼──────────┤
│    1     │ Taj Palace   │ Mumbai │   150    │
│    2     │ The Oberoi   │ Delhi  │    95    │
└──────────┴──────────────┴────────┴──────────┘
```

---

## 📚 Practical Questions

### Question 1: Table Creation
**File:** `Q1.md`

Create a Hotels table with the following specifications:
- `hotel_id` as PRIMARY KEY
- `hotel_name` as UNIQUE (VARCHAR 60)
- `city` (VARCHAR 40)
- `rooms_available` as NOT NULL (INT)

**Key Concepts:**
- Primary Key constraint
- Unique constraint
- NOT NULL constraint
- Data type selection

### Question 2: DML Operations
**File:** `Q2.md`

Perform various operations on the Hotels table:
- Insert two hotel records
- Update room availability
- Delete a hotel record
- Calculate total rooms (SUM)
- Calculate average rooms (AVG)

**Key Concepts:**
- INSERT statement
- UPDATE statement
- DELETE statement
- Aggregate functions (SUM, AVG)

---

## 🚀 Getting Started

### Prerequisites

- SQL Database Management System (MySQL, PostgreSQL, SQL Server, etc.)
- SQL Client or Command Line Interface

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd DBMS-PRATCTICAL
```

2. Open your SQL client and connect to your database

3. Execute the queries in order:
   - Start with `Q1.md` to create the table
   - Then run `Q2.md` to perform operations

### Example Usage

```sql
-- Step 1: Create the table (from Q1.md)
CREATE TABLE Hotels (
    hotel_id INT PRIMARY KEY,
    hotel_name VARCHAR(60) UNIQUE,
    city VARCHAR(40),
    rooms_available INT NOT NULL
);

-- Step 2: Insert data (from Q2.md)
INSERT INTO Hotels (hotel_id, hotel_name, city, rooms_available)
VALUES (1, 'Taj Palace', 'Mumbai', 120);
```

---

## 🔧 SQL Operations Covered

| Operation Type | SQL Command | Description |
|----------------|-------------|-------------|
| **DDL** | `CREATE TABLE` | Create database table structure |
| **DML** | `INSERT` | Add new records to table |
| **DML** | `UPDATE` | Modify existing records |
| **DML** | `DELETE` | Remove records from table |
| **DQL** | `SELECT SUM()` | Calculate total sum |
| **DQL** | `SELECT AVG()` | Calculate average value |

---

## 📊 Visual Summary

```
┌─────────────────────────────────────────────────────────┐
│                    SQL Operations Flow                   │
├─────────────────────────────────────────────────────────┤
│                                                          │
│  1. CREATE TABLE                                         │
│     └─▶ Define structure & constraints                  │
│                                                          │
│  2. INSERT INTO                                          │
│     └─▶ Add initial data                                │
│                                                          │
│  3. UPDATE                                               │
│     └─▶ Modify existing data                            │
│                                                          │
│  4. DELETE                                               │
│     └─▶ Remove records                                  │
│                                                          │
│  5. SELECT with Aggregates                               │
│     ├─▶ SUM() - Total calculation                       │
│     └─▶ AVG() - Average calculation                     │
│                                                          │
└─────────────────────────────────────────────────────────┘
```

---

## 🎓 Learning Outcomes

After completing these exercises, you will understand:

- ✅ How to create tables with proper constraints
- ✅ How to insert, update, and delete data
- ✅ How to use aggregate functions for calculations
- ✅ Best practices for SQL table design
- ✅ Importance of data integrity constraints

---

## 📝 Notes

- All SQL queries follow standard SQL syntax
- Queries are compatible with most SQL database systems
- Make sure to execute queries in the correct order
- Always verify constraints before inserting data

---

## 🤝 Contributing

Feel free to submit issues or pull requests if you find any improvements or have suggestions!

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

<div align="center">

**Made with ❤️ for DBMS Learning**

⭐ Star this repo if you find it helpful!

</div>
