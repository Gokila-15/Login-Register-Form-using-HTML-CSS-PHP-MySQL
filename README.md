# PHP Login & Register System

A simple user authentication system built with PHP, MySQL, and HTML/CSS. This project allows users to register, login, and be redirected to user-specific pages based on their role (Admin or User).

## 🚀 Features

- User registration with role selection (admin/user)
- Secure password hashing using `password_hash()`
- Login authentication with session management
- Redirect users to respective dashboards
- Error handling and form validations
- Logout functionality
- Clean and responsive UI

## 📁 Folder Structure

/login_register
│
├── config.php # Database connection
├── index.php # Login/Register form
├── login_register.php # Handles form submission
├── user_page.php # User dashboard
├── admin_page.php # Admin dashboard
├── logout.php # Logout logic
├── style.css # Styling
├── script.js # Form toggle logic
└── README.md # Project documentation


## 🛠️ Technologies Used

- PHP 8
- MySQL (XAMPP)
- HTML5 & CSS3
- JavaScript (basic)
- Apache server

## ⚙️ Setup Instructions

1. Clone this repository or download the ZIP.
2. Move the project folder to `htdocs` (if using XAMPP).
3. Start Apache and MySQL from XAMPP.
4. Create a MySQL database named `your_db_name` and import the users table:

sql
CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    email VARCHAR(100) NOT NULL UNIQUE,
    password VARCHAR(255) NOT NULL,
    role VARCHAR(50) NOT NULL
);
