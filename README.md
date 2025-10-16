# 🎓 Smart Student Result Management System (SRMS)

A **Student Result Management System (SRMS)** built using **PHP, MySQL, HTML, CSS, and Bootstrap**.  
This mini project helps colleges manage **departments, students, subjects, marks, and results** efficiently — all through a simple, responsive web interface.

---

## 📘 Project Overview
The **Smart Student Result Management System** is a web-based application that automates the process of managing student academic results.  
It eliminates manual calculation errors and simplifies data handling for different departments.

The system includes:
- Department management  
- Student management  
- Subject management  
- Marks entry and validation  
- Automatic result calculation (percentage + grade)  
- Individual student transcripts  

---

## ✨ Features

✅ **Department Management** – Add, edit, delete departments  
✅ **Student Management** – Add students department-wise  
✅ **Subject Management** – Assign subjects department-wise  
✅ **Marks Management** – Enter, update, and delete marks (auto-prevents duplicates)  
✅ **Result Generation** – Auto-calculate total marks, percentage, and grade  
✅ **Transcript View** – View individual subject-wise performance  
✅ **CSV Export** – Export student and result lists easily  
✅ **Responsive UI** – Built with Bootstrap 5 for all screen sizes  

---

## 🧠 Tech Stack

| Layer | Technology |
|--------|-------------|
| Frontend | HTML, CSS, Bootstrap 5 |
| Backend | PHP (Procedural) |
| Database | MySQL |
| Server | XAMPP (Localhost) / 000webhost (Live) |
| Version Control | Git & GitHub |

---

## 🧩 Database Design

**Database Name:** `student_result`

### Tables:
1. **departments** – department_id, dept_name  
2. **students** – student_id, name, roll_no, department_id, year  
3. **subjects** – subject_id, subject_name, subject_code, department_id, max_marks  
4. **marks** – mark_id, student_id, subject_id, marks_obtained  
5. **result** – result_id, student_id, total_marks, total_max, percentage, grade

**Relationships:**
- One Department → Many Students  
- One Department → Many Subjects  
- One Student → Many Marks  
- One Subject → Many Marks  
- One Student → One Result  

---



## ⚙️ Installation Guide (Local Setup)

### 🪟 Step 1 — Requirements
- Install **XAMPP**
- Start **Apache** and **MySQL**

### 💾 Step 2 — Database Setup
1. Open `http://localhost/phpmyadmin`
2. Create a new database named **`student_result`**
3. Import the provided SQL file (`student_result.sql`)

### 🧩 Step 3 — Project Setup
1. Copy the project folder to:

2. Edit `db.php` and update your local credentials:
```php
$DB_HOST = '127.0.0.1';
$DB_USER = 'root';
$DB_PASS = '';
$DB_NAME = 'student_result';

3. http://localhost/student_result_management/


