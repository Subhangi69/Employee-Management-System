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
- MySQL backend for persistent storage.
- Java Swing frontend for GUI.

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
### 3. Configure database connection
Create a db.properties file in the project root
```bash
db.url=jdbc:mysql://localhost:3306/employeemanagement
db.user=root
db.password=NewRootPass123!
```
### 4. Add required libraries
Make sure the following JARs are inside the lib/ folder:
- jcalendar-1.4.jar
- rs2xml.jar
- mysql-connector-java-8.0.33.jar
### Running the Application
Compile
```bash
javac -d bin -cp "lib\jcalendar-1.4.jar;lib\rs2xml.jar;lib\mysql-connector-j-8.0.33.jar" src\employee\management\system\*.java
```
Run
```bash
java -cp "bin;lib\jcalendar-1.4.jar;lib\rs2xml.jar;lib\mysql-connector-j-8.0.33.jar" employee.management.system.Login
```
Login Credentials
Username: admin
Password: admin


