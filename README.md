# Todo In-Memory Console Application

A simple command-line Todo application built with Python that stores tasks in memory. This application allows users to add, view, update, delete, and mark tasks as complete. All data is lost when the application exits.

## Features

- Add new tasks with title and description.
- View a list of all tasks, including their status.
- Update existing tasks (title and/or description).
- Delete tasks.
- Mark tasks as complete.

## Prerequisites

- Python 3.13+

## Setup and Run

1.  **Ensure Python is Installed**:
    Make sure you have Python 3.13 or newer installed on your system. You can download it from [python.org](https://www.python.org/).

2.  **Navigate to the Project Directory**:
    Open your terminal or command prompt and navigate to the root directory of this project.

    ```bash
    cd /path/to/Todo-In-Memory-Console-App
    ```
    (Replace `/path/to/Todo-In-Memory-Console-App` with the actual path where you've saved the project.)

3.  **Run the Application**:
    Execute the following command to start the Todo application:

    ```bash
    python -m todo_app.main
    ```

4.  **Interact with the Application**:
    Follow the on-screen menu prompts to manage your tasks.

## Data Persistence

Please note that this application stores all task data **only in memory**. This means that all your tasks will be lost when the application is closed or terminated unexpectedly.
