# Barishal Doctor Appointment System

A Java Swing desktop application connected to MySQL using JDBC. The application source creates the `barishal_doctor_db` database and its tables when it starts.

## Requirements
- JDK 17 or later
- Apache NetBeans
- XAMPP MySQL / MariaDB or MySQL Server
- MySQL Connector/J

## Setup in NetBeans
1. Install JDK 17 or later and start MySQL in XAMPP.
2. Download MySQL Connector/J and place its JAR in the `lib` folder, named `mysql-connector-j-26.10.0.jar`.
3. Open the project folder in NetBeans using File → Open Project.
4. Confirm the Connector/J JAR is listed in Project Properties → Libraries. If it is missing, add `lib/mysql-connector-j-26.10.0.jar`.
5. Run the project. The configured main class is `main`.

## Database
The Java source currently connects to `localhost:3306` as user `root` with an empty password and creates `barishal_doctor_db` plus its tables automatically. Change the connection settings in `src/main.java` if your local MySQL credentials differ. Do not commit real passwords.

## Note
The original project used a Connector/J JAR at an absolute path on another computer. That path is machine-specific, so this repository uses a relative `lib` path instead. The JAR itself is not included.
