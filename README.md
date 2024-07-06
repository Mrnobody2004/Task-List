# Task Management App

A simple Python-based task management application that allows users to add, remove, list, and recommend tasks based on their priority using a Naive Bayes classifier.

## Features

- **Add Task**: Add a new task with a specified priority (Low/Medium/High).
- **Remove Task**: Remove an existing task by its description.
- **List Tasks**: List all the current tasks.
- **Recommend Task**: Recommend a task based on its priority (randomly selects from high-priority tasks).

## Installation

1. **Clone the repository:**
    ```sh
    git clone https://github.com/yourusername/task-management-app.git
    ```
2. **Navigate to the project directory:**
    ```sh
    cd task-management-app
    ```
3. **Install the required dependencies:**
    ```sh
    pip install pandas scikit-learn
    ```

## Usage

1. **Run the application:**
    ```sh
    python task_management_app.py
    ```
2. **Follow the on-screen menu options to manage your tasks:**
    - Add Task
    - Remove Task
    - List Tasks
    - Recommend Task
    - Exit

## Project Structure

- `task_management_app.py`: The main application script.
- `tasks.csv`: A CSV file to store the tasks (auto-generated).

## Functions

### `add_task(description, priority)`

Adds a new task with the given description and priority. The task list is saved to `tasks.csv`, and the model is retrained.

### `remove_task(description)`

Removes the task with the given description from the task list and updates `tasks.csv`.

### `list_tasks()`

Prints all the current tasks. If no tasks are available, it notifies the user.

### `recommend_task()`

Recommends a high-priority task randomly from the list of tasks. If no high-priority tasks are available, it notifies the user.

## Contributing

Feel free to fork the repository and submit pull requests. Any contributions are welcome!

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

