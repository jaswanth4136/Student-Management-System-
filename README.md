# Student-Management-System-
A simple SQL project for managing student records, courses, and grades.

📌 Features
✅ Create a database and tables for students, courses, and grades.
✅ Insert sample student data and course details.
✅ Retrieve student information and grades using SQL queries.

🛠 Technologies Used
MySQL (or any SQL database)
📂 Project Structure

📦 SQL-Student-Management  
 ┣ 📜 schema.sql   → Defines database tables  
 ┣ 📜 data.sql     → Contains sample data  
 ┣ 📜 queries.sql  → Common SQL queries  
 ┗ 📜 README.md    → Project documentation  
 
🚀 How to Use
1️⃣ Setup the Database
Run the following command in MySQL to create the database and tables:


source schema.sql;
2️⃣ Insert Sample Data
Populate the database with sample records:


source data.sql;
3️⃣ Run SQL Queries
Test the predefined queries:


source queries.sql;
📊 Example Queries
🔹 List all students:


SELECT * FROM Students;
🔹 Find students in Computer Science:


SELECT * FROM Students WHERE department = 'Computer Science';
🔹 Fetch student grades:


SELECT Students.name, Courses.course_name, Grades.grade
FROM Grades
JOIN Students ON Grades.student_id = Students.student_id
JOIN Courses ON Grades.course_id = Courses.course_id;
