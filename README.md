# 💼 HireMind - Hiring & Job searching Platform 🤝

A **role-based hiring website** built using **Flask** and **MySQL**, enabling clients to hire workers for specific jobs, manage job requests, and track confirmations.

This project demonstrates **end-to-end full-stack web development**, including authentication, role management, relational database design, and CRUD workflows.

---

## 🔑 Features

### 👤 User Roles

#### **Client**

* Register and log in
* Search available workers
* Send hire requests
* View requested and confirmed jobs

#### **Worker**

* Register and log in
* Post job listings
* Accept or reject hire requests
* Close jobs and receive ratings

#### **Admin**

* Secure admin login
* System-wide overview access

---

### 🛠 Core Functionalities

* Session-based authentication
* Role-based access control
* Job search and filtering
* Hire request and acceptance workflow
* Worker rating system
* Relational MySQL database with foreign keys
* AJAX-based dynamic content loading

---

## 🧰 Tech Stack

| Layer      | Technology               |
| ---------- | ------------------------ |
| Backend    | Flask (Python)           |
| Database   | MySQL / MariaDB          |
| Frontend   | HTML, CSS, JavaScript    |
| ORM/Driver | PyMySQL                  |
| Server     | Flask Development Server |

---

## 🗄 Database Schema

The application uses the following tables:

* `client`
* `worker`
* `job`
* `requested`
* `accepted`

Relational constraints and cascading deletes are implemented to maintain data integrity.

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/HireMind-Hiring_-_Job_Searching_Platform.git
HireMind-Hiring_-_Job_Searching_Platform
```

---

### 2️⃣ Create a Virtual Environment (Recommended)

```bash
python -m venv venv
venv\Scripts\activate
```

---

### 3️⃣ Install Dependencies

```bash
pip install -r requirements(HireMind).txt
```

---

### 4️⃣ Set Up the Database

1. Open **phpMyAdmin**
2. Create a database:

```sql
CREATE DATABASE mamaar;
```

3. Import the provided `mamaar.sql` file

---

### 5️⃣ Configure Database Credentials

Edit `config.py`:

```python
DB_IP = 'localhost'
DB_USER = 'root'
DB_PASSWORD = ''
DATABASE = 'mamaar'
```

---

### 6️⃣ Run the Application

```bash
python app.py
```

Access the application at:

```
http://127.0.0.1:5000/
```

---

## 📸 Screenshots

Example:

```md
![Home Page](screenshots/demo.gif)
```

---

## ⚠️ Security Notes

* Passwords are stored in **plain text** (academic/demo purpose only)
* Not production-ready without:

  * Password hashing
  * CSRF protection
  * Input validation

---

## 🔮 Future Improvements

* Password hashing using Werkzeug
* Flask Blueprints for modular structure
* REST API architecture
* Pagination and advanced filtering
* Dockerized deployment
* JWT-based authentication

---
## 📜 License

This project is licensed for **educational and learning purposes only**.

---
