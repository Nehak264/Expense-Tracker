# 💸 Expense Tracker

A full-stack **Expense Tracker** web application built with **Java Spring Boot** for the backend, **MySQL** for persistent storage, and **HTML/CSS/JavaScript** for the frontend. Supports complete CRUD operations for managing personal expenses.

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Backend | Java, Spring Boot, Spring MVC |
| ORM | Spring Data JPA, Hibernate |
| Database | MySQL |
| Frontend | HTML, CSS, JavaScript |
| Build Tool | Maven |

---

## ✨ Features

- ➕ **Add** new expenses with title, amount, category, and date
- 📋 **View** all expenses in a clean, organized list
- ✏️ **Update** existing expense details
- 🗑️ **Delete** expenses you no longer need
- 💾 Persistent data storage using MySQL
- 🔗 RESTful API design with clean separation of concerns

---

## 📁 Project Structure

```
Expense-Tracker/
├── src/
│   └── main/
│       ├── java/com/example/expensetracker/
│       │   ├── controller/        # REST controllers (ExpenseController)
│       │   ├── model/             # Entity classes (Expense)
│       │   ├── repository/        # JPA repositories (ExpenseRepository)
│       │   ├── service/           # Business logic (ExpenseService)
│       │   └── ExpenseTrackerApplication.java
│       └── resources/
│           ├── static/
│           │   ├── css/
│           │   └── images/
│           ├── templates/
│           │   ├── index.html
│           │   ├── add-expense.html
│           │   └── update-expense.html
│           └── application.properties
├── pom.xml
└── README.md
```

---

## ⚙️ Getting Started

### Prerequisites

- Java 17+
- Maven 3.6+
- MySQL 8.0+
- Git

### 1. Clone the repository

```bash
git clone https://github.com/your-username/Expense-Tracker.git
cd Expense-Tracker
```

### 2. Configure the database

Create a MySQL database:

```sql
CREATE DATABASE expense_tracker;
```

Update `src/main/resources/application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/expense_tracker
spring.datasource.username=your_mysql_username
spring.datasource.password=your_mysql_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

### 3. Build and run

```bash
mvn spring-boot:run
```

### 4. Open in browser

```
http://localhost:8080
```


## 🔗 API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | `/expenses` | Get all expenses |
| GET | `/expenses/{id}` | Get expense by ID |
| POST | `/expenses/add` | Add a new expense |
| PUT | `/expenses/update/{id}` | Update an expense |
| DELETE | `/expenses/delete/{id}` | Delete an expense |

---

## 📚 What I Learned

- Building layered Spring Boot applications (Controller → Service → Repository)
- Using Spring Data JPA and Hibernate ORM for database interaction
- Designing and consuming REST APIs
- Connecting a frontend (HTML/CSS/JS) with a Spring Boot backend
- Managing database schema with `spring.jpa.hibernate.ddl-auto`

---

## 👨‍💻 Author

**Your Name**
- GitHub: 
- LinkedIn: https://www.linkedin.com/in/neha-kulkarni-99a207212/

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
