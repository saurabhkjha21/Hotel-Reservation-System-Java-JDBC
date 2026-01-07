# Hotel Reservation System (Java JDBC)

A console-based backend application built using **Java and JDBC** that performs real-time CRUD operations on a **MySQL database**.  
This project demonstrates core backend development concepts such as database connectivity, SQL operations, and clean code structure.

---

## Features

- Reserve a room by entering guest details
- View all reservations with complete information
- Update existing reservation details
- Delete reservations using reservation ID

---

## Tech Stack

- Java (JDK 17+)
- JDBC
- MySQL
- IntelliJ IDEA
- Git & GitHub

---

## Database Setup

```sql
CREATE DATABASE hotel_db;

USE hotel_db;

CREATE TABLE reservations (
    reservation_id INT AUTO_INCREMENT PRIMARY KEY,
    guest_name VARCHAR(50) NOT NULL,
    room_number INT NOT NULL,
    contact_number VARCHAR(15) NOT NULL,
    reservation_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);


Project Structure
Hotel-Reservation-System-Java-JDBC
│
├── src/
│   ├── HotelReservationSystem.java
│   └── Main.java
├── .gitignore
└── README.md

How to Run

Clone the repository:

git clone https://github.com/saurabhkjha21/Hotel-Reservation-System-Java-JDBC.git


Open the project in IntelliJ IDEA

Add MySQL Connector/J to the project dependencies

Update database credentials in HotelReservationSystem.java:

private static final String url = "jdbc:mysql://localhost:3306/hotel_db";
private static final String username = "root";
private static final String password = "your_password";


Run the application:

java HotelReservationSystem


Notes

This is a console-based application

Uses JDBC for database connectivity

Data is stored persistently in MySQL

Designed for learning backend fundamentals

Future Enhancements

Use PreparedStatement to prevent SQL Injection

Implement DAO design pattern

Convert to Spring Boot REST APIs

Add authentication and web UI

Author

Saurabh Kumar Jha
MCA Student | Java Backend Developer

GitHub: https://github.com/saurabhkjha21

LinkedIn: https://www.linkedin.com/in/saurabhkjha21/
