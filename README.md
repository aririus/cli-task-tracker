# CLI Task Tracker 📝

A simple command-line application for tracking your tasks — built with pure Python and no external libraries.

## ✨ Features

- Add a task
- List all tasks or by status (`todo`, `in-progress`, `done`)
- Update a task's description
- Delete a task
- Mark tasks as in-progress or done
- Data stored in a local JSON file

## 🛠 Tech Stack

- Python 3
- Standard Library only (`sys`, `os`, `json`, `datetime`)

## 🚀 How to Install

1. Clone the repo:
   ```bash
   git clone https://github.com/aririus/cli-task-tracker.git
   cd cli-task-tracker
2. Make the script executable:
   ```bash
   chmod +x tracker-cli
3. (Optional) Add an alias to your shell config:
   ```bash
   alias tracker-cli="$PWD/tracker-cli"
4. Now you can run:
   ```bash
   tracker-cli add "Finish the project"

## 🧑‍💻 Example Usage

```bash
tracker-cli add "Read a book"
# Output: Task added successfully (ID:1)

tracker-cli list
# Output:
# ID: 1
# Description: Read a book
# Status: todo
# Created At: 2025-05-16T10:29:35.354108
# Updated At: 2025-05-16T10:29:35.354108
# ----------------------------------------

tracker-cli list done
# Output: No tasks found

tracker-cli update 1 "Read two books"
# Output: Task 1 updated successfully

tracker-cli mark-in-progress 1
# Output: Task 1 marked as in-progress

tracker-cli mark-done 1
# Output: Task 1 marked as done

tracker-cli delete 1
# Output: Task 1 deleted successfully
```

