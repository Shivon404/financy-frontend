# 💰 FINANCY - Student Finance Tracker

A full-stack web application designed to help students manage their finances by tracking expenses, setting budgets, and monitoring spending habits.

## 📸 Features

- ✅ User Registration & Authentication
- ✅ Expense Management (Add, Edit, Delete)
- ✅ Budget Setting by Category with Alerts
- ✅ Real-time Budget Tracking & Warnings
- ✅ User Profile with Statistics
- ✅ Edit Monthly Allowance
- ✅ Dashboard with Summary Cards
- ✅ Expense History & Reports

## 🛠️ Tech Stack

### Frontend
- HTML5
- CSS3
- Vanilla JavaScript

### Backend
- C# (.NET 8 Web API)
- Object-Oriented Programming (OOP)
- RESTful API Architecture

### Database
- MySQL
- Relational Database Design

### Tools
- Visual Studio Code
- XAMPP (MySQL)
- Git & GitHub

## 📂 Project Structure
```
Financy/
├── Frontend/
│   ├── index.html          # Login & Registration
│   └── dashboard.html      # Main Dashboard
│
└── FinancyAPI/
    ├── Controllers/        # API Endpoints
    │   ├── AuthController.cs
    │   ├── ExpenseController.cs
    │   └── BudgetController.cs
    │
    ├── Models/            # Data Models (OOP)
    │   ├── User.cs
    │   ├── Expense.cs
    │   ├── Budget.cs
    │   └── Category.cs
    │
    ├── Services/          # Business Logic Layer
    │   ├── DatabaseService.cs
    │   ├── UserService.cs
    │   ├── ExpenseService.cs
    │   └── BudgetService.cs
    │
    └── DTOs/              # Data Transfer Objects
        ├── LoginRequest.cs
        └── RegisterRequest.cs
```

## 🚀 Setup Instructions

### Prerequisites
- [.NET 8 SDK](https://dotnet.microsoft.com/download)
- [XAMPP](https://www.apachefriends.org/) (for MySQL)
- Visual Studio Code

### Database Setup

1. Start XAMPP and run MySQL
2. Open phpMyAdmin (`http://localhost/phpmyadmin`)
3. Create `financy_db` database
4. Run the SQL script to create tables

### Backend Setup
```bash
cd FinancyAPI
dotnet restore
dotnet run
```

Backend will run on: `http://localhost:5290`

### Frontend Setup

Simply open `Frontend/index.html` in your browser!

Or use Live Server in VS Code:
1. Install "Live Server" extension
2. Right-click `index.html` → "Open with Live Server"

## 🧪 Test Account

- **Email:** test@student.com
- **Password:** test123

## 📊 Database Schema

### Users
- user_id, first_name, last_name, email, password, student_id, monthly_allowance, created_at

### Expenses
- expense_id, user_id, category_id, amount, expense_date, description, created_at

### Budgets
- budget_id, user_id, category_id, budget_limit, month, created_at

### Categories
- category_id, category_name, icon

## 🎯 OOP Principles Applied

- **Encapsulation:** Data and methods grouped in classes
- **Abstraction:** Service layer abstracts database operations
- **Separation of Concerns:** Controllers, Services, Models, DTOs
- **Dependency Injection:** Services injected into controllers

## 👥 Team

OOP Final Project

## 📝 License

This project is for educational purposes.
```

---

## So in VS Code:

1. **Create file `.gitignore`** → Copy the FIRST code block above → Paste it → Save
2. **Create file `README.md`** → Copy the SECOND code block above → Paste it → Save

---

## Your Financy folder should now have:
```
Financy/
├── .gitignore       ← NEW FILE YOU JUST CREATED
├── README.md        ← NEW FILE YOU JUST CREATED
├── Frontend/
│   ├── index.html
│   └── dashboard.html
└── FinancyAPI/
    └── (all your backend files)