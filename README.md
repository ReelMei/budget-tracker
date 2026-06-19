# Campus Budget Tracker

A simple web-based budget management application built for students to track their income and expenses. The application allows users to record financial transactions, calculate their balance, and manage their spending habits.

The project was developed using **Python, Flask, SQLite, and SQLAlchemy**.

---

## Features

- Add income records
- Add expense records
- View all transactions
- Automatically calculate:
  - Total income
  - Total expenses
  - Current balance
- Categorize transactions
- Delete transactions
- Store data permanently using SQLite database

---

## Technologies Used

### Backend
- Python
- Flask
- Flask-SQLAlchemy

### Database
- SQLite

### Frontend
- HTML
- CSS
- Jinja2 Templates

### Development Tools
- Git
- GitHub
- Virtual Environment (venv)

---

## System Architecture

The application follows a simple three-layer architecture:

### Explanation

- **User Layer:** The student interacts with the web interface.
- **Application Layer:** Flask handles requests, processes data, and controls application logic.
- **Database Layer:** SQLite stores transaction records permanently.

---

## Project Structure
campus-budget-tracker/
│
├── app.py                       # Main Flask application
├── requirements.txt             # Python dependencies
├── README.md                    # Project documentation
├── budget.db                    # SQLite database file
├── .gitignore                   # Files Git should ignore
│
├── templates/                   # HTML files (Jinja2 templates)
│   │
│   ├── index.html               # Dashboard/home page
│   └── add_transaction.html     # Add income/expense form
│
├── static/                      # Static files (CSS)
│   │
│   ├── css/
│       └── style.css            # Website styling
│ 
│   
│
└── venv/                        # Python virtual environment (NOT pushed to GitHub)


## Database Design

The application uses a `Transaction` table.

| Column | Data Type | Description |
|--------|-----------|-------------|
| id | Integer | Unique transaction identifier |
| title | String | Name of transaction |
| amount | Float | Money value |
| type | String | Income or expense |
| category | String | Transaction category |
| date | DateTime | Date transaction was created |

---

## Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/ReelMei/budget-tracker.git