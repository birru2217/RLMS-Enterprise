<div align="center">
  <img src="[INSERT_LOGO_IMAGE_LINK_HERE]" alt="RLMS Logo" width="150"/>
  <h1>🎓 Registration & Learning Management System (RLMS)</h1>
  <p><strong>An Enterprise-Grade, 5-Tier Educational Ecosystem</strong></p>

  <!-- Tech Stack Badges -->
  <p>
    <img src="https://img.shields.io/badge/PHP-8.x-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP">
    <img src="https://img.shields.io/badge/MySQL-Database-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL">
    <img src="https://img.shields.io/badge/JavaScript-Vanilla-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JS">
    <img src="https://img.shields.io/badge/AJAX-RealTime-005C84?style=for-the-badge" alt="AJAX">
    <img src="https://img.shields.io/badge/Security-2FA_Enabled-DC2626?style=for-the-badge&logo=springsecurity" alt="Security">
  </p>
</div>

<hr>

## 🌟 Project Overview
**RLMS (Registration & Learning Management System)**, evolved from the EPLMS concept, is a highly secure, automated, and unified academic platform engineered for **Bule Hora University**. It completely digitizes the academic workflow—from student registration to secure exam processing and auto-calculating gradebooks.

### 🔭 The Grand Vision (Zero-Data Access)
The ultimate architectural goal of this project is to partner with **Ethio-Telecom**. Similar to how *Telebirr* operates seamlessly without active internet data, RLMS is designed with the potential to function as an offline, **zero-data educational portal**, eliminating financial barriers for university students across Ethiopia.

<div align="center">
  <!-- 📸 SCREENSHOT 1: CONTROL CENTER / DASHBOARD -->
  <img src="[INSERT_IMAGE_LINK_HERE_FOR_DASHBOARD]" alt="Super Admin Dashboard" width="800" style="border-radius: 10px; box-shadow: 0 10px 20px rgba(0,0,0,0.2);">
  <br>
  <em>Figure 1: Super Admin SPA Control Center with Live Demographics.</em>
</div>

---

## 🏛️ The 5-Tier RBAC Architecture
The system is built on a strict **Role-Based Access Control (RBAC)** hierarchy to ensure data privacy and operational efficiency.

1. 👑 **Super Admin:** Global system owner. Manages colleges, global security logs, and social configurations.
2. 🏛️ **College Admin:** Campus-level manager. Creates departments, assigns Heads, and sets up public mail servers.
3. 👥 **Department Head:** Departmental authority. Approves student registrations seamlessly, assigns courses, and manages faculty.
4. 👨‍🏫 **Teacher:** Course instructor. Uploads study materials (with auto-release dates), schedules secure exams, and manages the gradebook.
5. 🎓 **Student:** The end-user. Registers via secret codes, accesses courses, submits assignments, takes timed exams, and tracks grades.

<div align="center">
  <!-- 📸 SCREENSHOT 2: SPA OVERSIGHT / HIERARCHY DRILL-DOWN -->
  <img src="[INSERT_IMAGE_LINK_HERE_FOR_SPA_OVERSIGHT]" alt="SPA Drill-Down Oversight" width="800" style="border-radius: 10px; box-shadow: 0 10px 20px rgba(0,0,0,0.2);">
  <br>
  <em>Figure 2: Single Page Application (SPA) Drill-Down Department Oversight.</em>
</div>

---

## 🚀 Key Features

### 🛡️ Military-Grade Cybersecurity
- **2-Factor Authentication (2FA):** Mandatory OTP verification via SMTP email for logins.
- **Anti-Brute Force (Auto-Banning):** Automatically bans attacker IPs for 24 hours after 3 failed attempts.
- **Audit Logging:** Live tracking of all authentication attempts with device and IP detection.
- **Profile Privacy:** Users can lock their avatars to maintain a strictly professional presence.

### 🧠 Smart Examination Engine
- **Server-Time Sync:** Exams open and close strictly based on PHP server time, ignoring client-side manipulation.
- **Secret Access Codes:** Students require dynamic codes provided by instructors to enter the exam gateway.
- **Anti-Cheat Mechanics:** Instantly detects tab-switching and triggers a "Screen Blackout" if screenshots (e.g., *PrtScn*, *Win+Shift+S*) are attempted.
- **Auto-Submission:** Automatically submits the exam when the timer hits zero.
- **AI Auto-Grading:** Instantly grades multiple-choice and fill-in-the-blank questions, with a delayed results release to prevent cheating.

<div align="center">
  <!-- 📸 SCREENSHOT 3: EXAM ENGINE / ANTI-CHEAT -->
  <img src="[![Uploading $REPE999.png…]()
]" alt="Secure Exam Engine" width="800" style="border-radius: 10px; box-shadow: 0 10px 20px rgba(0,0,0,0.2);">
  <br>
  <em>Figure 3: Secure Exam Engine with Pagination and Live Countdown Timer.</em>
</div>

### 💬 Encrypted AJAX Communications Hub
- A built-in, native "Telegram-style" chat interface.
- Supports **Private 1-on-1 Chats** and **Role-restricted Group Broadcasts** (e.g., Head to Teachers, Teacher to Students).
- Real-time fetching without page reloads using optimized AJAX intervals.

<div align="center">
  <!-- 📸 SCREENSHOT 4: CHAT / COMMUNICATIONS HUB -->
  <img src="[INSERT_IMAGE_LINK_HERE_FOR_CHAT]" alt="Encrypted Chat Hub" width="800" style="border-radius: 10px; box-shadow: 0 10px 20px rgba(0,0,0,0.2);">
  <br>
  <em>Figure 4: The Internal AJAX-Powered Communication Hub.</em>
</div>

### 📊 Automated Master Gradebook
- Teachers can set custom weights (e.g., Mid 20%, Final 30%).
- The system automatically calculates total percentages and generates Letter Grades (A, B, C...).
- **Publish Mode:** Once published, grades are locked and instantly available to students and the HoD.

---

## 💻 Tech Stack
- **Frontend:** HTML5, CSS3 (Custom Glassmorphism UI), Vanilla JavaScript, Chart.js.
- **Backend:** PHP 8.x (Vanilla, Procedural & OOP components).
- **Database:** MySQLi (Highly normalized with `ON DELETE CASCADE` constraints).
- **Third-Party Libraries:** [PHPMailer](https://github.com/PHPMailer/PHPMailer) for secure SMTP integration.

---

## ⚙️ Installation & Setup
To run this project locally, follow these steps:

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/birru2217/RLMS-Enterprise.git
