# Flask TODO Application

This is a simple Todo application built using Flask, SQLAlchemy, and JavaScript. It allows users to add, view, update, and delete tasks. Tasks can also be marked as completed or incomplete using the ❌ and ✔️ signs.

## Table of Contents

- [Getting Started](#getting-started)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Routes](#routes)
- [Contributing](#contributing)

## Getting Started

To get started with this TODO application, follow the steps in the [Installation](#installation) section. Once the application is up and running, you can access it in your web browser at `http://localhost:8000/`.

## Prerequisites

Before running the application, ensure you have the following installed on your system:

- Python 3 (https://www.python.org/downloads/)
- Flask (latest version)
- SQLAlchemy (latest version)

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/flask-todo-app.git
   cd flask-todo-app

2. Create the SQLite database by running the following commands:

   ```bash
    from app import db
    db.create_all()
    exit()

  
4. Run the application:
   ```bash
    python app.py

## Usage

- Access the application in your web browser at http://localhost:8000/.
- To add a new task, enter the task title and description in the "Add a Todo" form and click the "Submit" button.
-  All your todos will be displayed in a table with columns for "SNo," "Title," "Description," "Status," and "Time."
- To update a task, click the "Update" button in the corresponding row and enter the updated title and description in the form that appears.
- To delete a task, click the "Delete" button in the corresponding row.
- To mark a task as completed or incomplete, click the ❌ or ✔️ sign in the "Status" column. The sign will toggle between the two states.

## Routes

- /: Home page to view and manage TODO items.
- /show: Testing route to view all TODO items in the database.
- /update/<int:sno>: Route to update a specific TODO item based on its serial number (sno).
- /delete/<int:sno>: Route to delete a specific TODO item based on its serial number (sno).

## Contributing

Contributions are welcome! If you find any bugs or have suggestions for improvements, please open an issue or submit a pull request.
