# Employee Management System (Java + MySQL)

A desktop-based **Employee Management System** built using **Java Swing** and **MySQL**.  
This application allows users to log in, add new employees, view records, and remove employees.  
It demonstrates the integration of Java GUI with a relational database using **JDBC**.

---

## Features
- Secure login system (default: `admin` / `admin`).
- Add employee details (name, DOB, salary, address, phone, email, etc.).
- View all employees in a tabular format.
- Remove employees by ID.
## Tech Stack
Java Swing – UI
- MySQL – Database
- JDBC – Database connectivity
- JCalendar & rs2xml – Date picker & table model utilities

---

## Prerequisites
Make sure you have the following installed:
- [Java JDK 17+]
- [MySQL Server]
- Git (to clone the repository).

---

## Setup Instructions

### 1. Clone this repository
```bash
git clone https://github.com/your-username/Employee-Management-System.git
cd Employee-Management-System
```
### 2. Setup the database
Run the provided SQL script to create the required schema and tables:
```bash
mysql -u root -p < sql/setup.sql
```
This will:
- Create database employeemanagement
- Create table login with a default admin user (admin / admin)
- Create table employee for storing employee details

