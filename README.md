# Sql-Student-Management
CREATE DATABASE student_db;

USE student_db;

CREATE TABLE students (
    student_id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100) NOT NULL,
    age INT,
    course VARCHAR(50),
    email VARCHAR(100) UNIQUE,
    marks DECIMAL(5,2)
);

INSERT INTO students (name, age, course, email, marks)
VALUES
('Ram', 21, 'BCA', 'ram@gmail.com', 85.50),
('Shyam', 20, 'BCA', 'shyam@gmail.com', 92.00);

SELECT * FROM students;

