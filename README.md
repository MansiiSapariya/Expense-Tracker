# Budget Buddy – Expense Tracker

A full-stack personal finance management web application that allows users to securely manage income and expenses, maintain transaction records, and visualize their spending patterns.

## About the Project

**Budget Buddy** is an expense tracker website developed as a Full Stack Web Development project.

The application provides users with a centralized platform to:

* Create and manage user accounts
* Log in securely
* Record income and expenses
* Edit and delete transactions
* View transaction history
* Categorize transactions
* Analyze spending patterns using interactive visualizations

The project demonstrates the integration of frontend development, backend application logic, database management, authentication, and data visualization in a single web application. 

## Features

### User Account Management

Users can register and log in to their accounts using their credentials.

The application includes:

* User registration
* Login authentication
* Session management
* Password hashing
* Logout functionality

The backend uses Flask sessions and password hashing for authentication. 

### Transaction Management

Users can manage their financial transactions by:

* Adding transactions
* Recording income and expenses
* Selecting transaction categories
* Adding dates and descriptions
* Editing existing transactions
* Deleting transactions

The transaction history page provides a detailed view of recorded transactions, including date, category, amount, and description. 

### Expense Visualization

Budget Buddy provides graphical representations of users' financial activity.

The project uses **Plotly** to create interactive visualizations that help users understand their spending behavior.

The report describes dynamic graphs and charts for displaying expenses over selected periods. 

### Responsive Interface

The application is designed to work across:

* Desktop
* Tablet
* Mobile devices

The project emphasizes usability and responsive interface design. 

---

## Technology Stack

### Backend

* Python
* Flask
* Flask-MySQLdb
* WTForms

### Frontend

* HTML
* CSS
* JavaScript
* Bootstrap
* jQuery

### Database

* MySQL

### Data Visualization

* Plotly

### Security

* Flask sessions
* Password hashing
* `itsdangerous`
* `passlib`
* Werkzeug security utilities

The application code uses Flask with MySQL connectivity and Plotly for visualization. 

---

## Application Workflow

```text
User Registration
       ↓
User Login
       ↓
Dashboard
       ↓
Add Income / Expense
       ↓
Store Transaction in MySQL
       ↓
View Transaction History
       ↓
Edit / Delete Transactions
       ↓
Analyze Spending
       ↓
Interactive Visualizations
```

---

## Project Structure

```text
budget-buddy-expense-tracker/
│
├── README.md
├── requirements.txt
├── .gitignore
├── config.py
├── config.example.py
├── app.py
├── queries.sql
│
├── templates/
│   ├── layout.html
│   ├── index.html
│   ├── about.html
│   ├── login.html
│   ├── signUp.html
│   ├── addTransactions.html
│   ├── transactionHistory.html
│   ├── editTransaction.html
│   ├── thank_you.html
│   │
│   └── includes/
│       ├── _navbar.html
│       ├── _messages.html
│       └── _formhelpers.html
│
├── static/
│   ├── css/
│   ├── js/
│   └── images/
│
└── docs/
    └── Project_Report_Full_Stack_Web_Development.pdf
```

---

## Getting Started

### Prerequisites

Make sure you have the following installed:

* Python 3.x
* MySQL
* pip

### 1. Clone the Repository

```bash
git clone https://github.com/<your-username>/budget-buddy-expense-tracker.git
```

Navigate to the project directory:

```bash
cd budget-buddy-expense-tracker
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

On macOS/Linux:

```bash
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure MySQL

Create the required MySQL database and tables using the SQL queries provided in:

```text
queries.sql
```

### 5. Configure the Application

Copy the example configuration:

```bash
copy config.example.py config.py
```

On macOS/Linux:

```bash
cp config.example.py config.py
```

Open `config.py` and add your own local database credentials.

**Do not commit `config.py` to GitHub.**

The actual configuration file is excluded through `.gitignore`.

### 6. Run the Application

```bash
python app.py
```

The application can then be accessed through the local Flask development server.

---

## Security

The project originally uses database and application configuration values through `config.py`.

For security, **real credentials should never be committed to GitHub**.

The repository includes:

```text
config.example.py
```

as a safe configuration template.

Your local:

```text
config.py
```

is excluded through:

```text
.gitignore
```

Before publishing the repository, make sure no real database passwords, API keys, email passwords, or secret keys are present in tracked files.

---

## Database

The application uses MySQL to store user and transaction information.

The backend establishes a MySQL connection through Flask-MySQLdb and performs database operations for user registration and transaction management. 

The SQL structure and queries used by the project are available in:

```text
queries.sql
```

---

## Challenges and Learnings

The project provided practical experience in several areas of full-stack development.

Key challenges included:

* Integrating frontend and backend functionality
* Implementing secure user authentication
* Connecting Flask with MySQL
* Creating dynamic financial visualizations
* Maintaining responsive user interfaces
* Testing the application workflow
* Balancing functionality with user experience

These challenges helped develop practical skills in full-stack application development, debugging, problem-solving, and user-centered design. 

---

## Future Scope

The project can be extended with additional financial management features, including:

* Budget planning
* Financial goal tracking
* Multi-currency support
* More advanced spending analytics
* Improved reporting
* Additional visualization options
* More detailed financial summaries

The original project also identifies budget planning, goal setting, and multi-currency support as possible future enhancements. 

---

## Documentation

The complete project report is available in:

```text
docs/Project_Report_Full_Stack_Web_Development.pdf
```

The report contains the project's:

* Introduction
* Objectives
* Scope
* System design
* Implementation
* Application screenshots
* Challenges and learnings
* Conclusion

---

## Project Scope

Budget Buddy is designed as a practical personal finance management application.

Its main scope includes:

* User account management
* Transaction recording
* Category management
* Expense visualization
* Responsive web design
* Extensibility for future financial features



---

## Author

**Mansi Sapariya**

Full Stack Web Development Project

---

## Disclaimer

This project was developed for academic and educational purposes. It is intended to demonstrate full-stack web development concepts and should not be considered a professional financial management or advisory service.
