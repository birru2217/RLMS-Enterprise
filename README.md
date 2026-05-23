# 🎓 RLMS - Registration & Learning Management System
![PHP](https://img.shields.io/badge/PHP-8.x-777BB4?style=for-the-badge&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-Database-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

**RLMS (Enterprise Edition)** is a highly secure, 5-tier architecture academic management platform designed to digitize the entire workflow of universities. It is currently engineered with the vision of providing a unified digital ecosystem for **Bule Hora University**.

## 🚀 Key Features
- **5-Tier Hierarchy:** Super Admin, College Admin, Dept Head, Teacher, and Student workflows.
- **Smart Exam Engine:** Server-time synchronized exams with Anti-Cheat mechanisms (Blackout on screenshot, Tab-switching detection).
- **Military-Grade Security:** 2-Factor Authentication (OTP via SMTP), and IP Auto-banning for brute-force defense.
- **Encrypted Communications:** A built-in, Telegram-style AJAX messaging hub for role-restricted private chats and broadcasts.
- **Dynamic Master Gradebook:** Auto-calculating assessments and instant letter-grade distribution.
- **Future Vision (All-In-One System):** Future updates will integrate Library Management, Dormitory Management, and an eventual partnership with Ethio-Telecom for **Zero-Data Offline Access**.

## 🛠️ Technologies Used
- **Frontend:** HTML5, CSS3 (Glassmorphism UI), Vanilla JavaScript, Chart.js, FontAwesome.
- **Backend:** Vanilla PHP 8.x
- **Database:** MySQLi (Highly normalized relational structure)
- **Security:** PHPMailer for OTP delivery.

## 📦 Installation Guide
1. Clone this repository: `git clone https://github.com/YourUsername/RLMS-Enterprise.git`
2. Move the folder to your local server directory (e.g., `htdocs` for XAMPP or `www` for WAMP).
3. Create a database named `eplms_db` in phpMyAdmin.
4. Import the provided SQL dump file into `eplms_db`.
5. Configure your database settings in `/includes/config.php`.
6. Configure your SMTP App Password in the Admin/Head dashboard settings for 2FA to work.
7. Run the project in your browser: `http://localhost/rlms`

## 🔐 Default Logins
*(Note: Change these immediately after installation)*
- **Super Admin:** Username: `superadmin` | Password: `@Biruk2217`

## 👨‍💻 Developer
Developed with passion and clean code architecture.

---
*“Empowering education through seamless technology.”*
