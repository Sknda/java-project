# Student Management Application

This is a simple student management application built using Java Swing for the frontend and JDBC with MySQL for the backend. The application allows users to add, update, delete, and retrieve student data.

## Features

- Add new student records
- Update existing student records
- Delete student records
- Retrieve and display all student records

## Prerequisites

- Java Development Kit (JDK) 8 or higher
- MySQL Database
- MySQL Connector/J (JDBC Driver for MySQL)

## Database Setup

1. Install MySQL and create a database named `student_db`.
2. Create a table named `students` using the following SQL script:

    ```sql
    CREATE DATABASE student_db;

    USE student_db;

    CREATE TABLE students (
        id INT AUTO_INCREMENT PRIMARY KEY,
        name VARCHAR(100) NOT NULL,
        age INT NOT NULL,
        major VARCHAR(100) NOT NULL
    );
    ```

3. Insert some sample data into the `students` table (optional):

    ```sql
    INSERT INTO students (name, age, major) VALUES
    ('Alice', 20, 'Computer Science'),
    ('Bob', 22, 'Mechanical Engineering'),
    ('Charlie', 21, 'Mathematics');
    ```

## Project Structure

