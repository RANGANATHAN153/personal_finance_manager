# personal_finance_manager
This repository contains a data analytics project, including datasets, preprocessing, EDA, visualizations, and insights using Python.
# Personal Finance Manager (Python CLI Project)

## Project Overview

The Personal Finance Manager is a command-line based Python application designed to help users track and analyze their daily expenses. The system allows users to add expenses, store them in a CSV file, generate financial reports, and analyze spending patterns.

This project demonstrates key programming concepts such as:

* Object-Oriented Programming (OOP)
* File Handling with CSV
* Data Persistence
* Error Handling
* Command-Line Interface (CLI)
* Basic Financial Data Analysis

The application stores expenses permanently and allows users to retrieve and analyze them anytime.

---

# Features

### Expense Management

* Add new expenses
* View all expenses
* Store expense data in CSV format

### Data Analysis

* Category-wise spending summary
* Monthly expense reports
* Search expenses by description

### Data Management

* Automatic data saving
* Backup and restore functionality
* Persistent storage using CSV files

### User Interface

* Interactive command-line menu
* Simple and user-friendly navigation
* Input validation and error handling

---

# Technologies Used

* **Python 3**
* **CSV module**
* **Object-Oriented Programming**
* **Google Colab / VS Code**

Optional tools used for development:

* GitHub for version control
* Jupyter Notebook / Colab for testing

---

# Project Structure

```
personal-finance-manager

main.py
README.md
requirements.txt

data/
    expenses.csv

src/
    expense.py
    file_manager.py
    reports.py
    utils.py

docs/
    user_guide.md

screenshots/
    menu.png
    reports.png
```

---

# Installation Guide

## Step 1: Install Python

Download Python from
https://www.python.org/downloads/

Verify installation:

```
python --version
```

---

## Step 2: Clone Repository

```
git clone https://github.com/yourusername/personal-finance-manager.git
```

Navigate to the project folder:

```
cd personal-finance-manager
```

---

## Step 3: Run the Application

Run the main program:

```
python main.py
```

The command-line interface menu will appear.

---

# How to Use the Program

When the program starts, the following menu will appear:

```
PERSONAL FINANCE MANAGER

1 Add Expense
2 View Expenses
3 Category Report
4 Monthly Report
5 Search Expense
6 Backup Data
7 Exit
```

### Add Expense

Enter the following details:

* Amount
* Category
* Date
* Description

Example:

```
Amount: 500
Category: Food
Date: 2026-03-14
Description: Lunch
```

---

### View Expenses

Displays all stored expenses with:

```
Date | Category | Amount | Description
```

Example:

```
2026-03-10 | Food | ₹250 | Lunch
2026-03-10 | Transport | ₹1200 | Taxi
```

---

### Category Report

Displays total spending per category.

Example:

```
Food: ₹250
Transport: ₹2900
Entertainment: ₹500
Shopping: ₹1000
```

---

### Monthly Report

Shows total expenses grouped by month.

Example:

```
2026-03 : ₹4650
```

---

### Search Expenses

Search expenses by keyword in the description.

Example:

```
Search keyword: lunch
```

Result:

```
2026-03-10 | Food | ₹250 | Lunch
```

---

### Backup Data

Creates a backup copy of the expense file.

```
backup_expenses.csv
```

---

# Example Dataset

Example CSV format:

```
Date,Category,Amount,Description
2026-03-10,Food,250,Lunch
2026-03-10,Transport,1200,Taxi
2026-03-04,Entertainment,500,Movie
```

---

# Technical Implementation

## Object-Oriented Design

The project uses an `Expense` class to represent expense records.

```
class Expense:
    def __init__(self, amount, category, date, description):
        self.amount = amount
        self.category = category
        self.date = date
        self.description = description
```

---

## File Handling

Expense data is stored using the Python **CSV module**.

Operations include:

* Reading CSV files
* Writing CSV files
* Data persistence
* Backup creation

---

# Error Handling

The application includes validation for:

* Invalid numeric values
* Missing inputs
* File reading errors
* Incorrect menu selections

---

# Screenshots

Menu Interface

```
PERSONAL FINANCE MANAGER
1 Add Expense
2 View Expenses
3 Category Report
4 Monthly Report
5 Search Expense
6 Backup Data
7 Exit
```

Expense Report Example

```
Category Summary
Food: ₹250
Transport: ₹2900
Shopping: ₹1000
```

---

# Future Improvements

Possible improvements include:

* Graphical User Interface (GUI)
* Data visualization charts
* Budget alerts
* Expense prediction using Machine Learning
* Database integration (MySQL or SQLite)
* Web application version

---

# Learning Outcomes

This project helps developers learn:

* Python programming fundamentals
* Object-Oriented Programming
* File handling and persistence
* Data organization and reporting
* CLI application development

---

# Author

Ranganathan
Data Analyst

---

# License

This project is for educational purposes.
