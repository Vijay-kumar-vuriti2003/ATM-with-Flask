# ATM-with-Flask
# ATM Web Application

This is a simple ATM banking simulation web app built using Python (Flask) and MySQL. It allows users to:
- Withdraw money
- Deposit money
- View mini statements
- Generate ATM PINs

## 🔧 Tech Stack

- Backend: Python (Flask)
- Database: MySQL
- Frontend: HTML (rendered via Flask templates)

## 📁 Project Structure

- app.py: Main Flask application with route handling
- sample.sql: SQL script to create and populate the `ACCOUNTS` table
- templates/: HTML files for the user interface (e.g. `home.html`, `withdraw1.html`, etc.)

## 🛠️ Setup Instructions

1. Clone the repository
2. Set up the MySQL database:

```bash
mysql -u root -p < sample.sql

## install dependencies:
pip install flask pymysql

## Default database credentials are set in app.py. Make sure they match your local setup:
db_config = {
    "host": "localhost",
    "user": "root",
    "password": "vijay",
    "database": "atm"
}
Sample users are available in sample.sql with some having no PIN set initially.

## 📷 Screens (HTML Templates)
Ensure the following templates are present in your templates/ folder:
home.html
withdraw1.html, withdraw2.html
deposit1.html
ministatement1.html, ministatement2.html
pingeneration1.html, pingeneration2.html
