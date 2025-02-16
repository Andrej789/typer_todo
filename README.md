# Command Line To-Do App with Python and Typer

This project is a command-line interface (CLI) application built using Python and Typer. It allows users to manage their to-do list efficiently through CLI commands. 

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Commands](#commands)
- [Usage](#usage)

---

## Features

- **User-Friendly CLI**: Clean and intuitive commands for managing to-do items.
- **Database**: Stores tasks in a JSON file as to-do database for persistence.
- **TODO Management**:
  - Add to-do with optional priority levels.
  - List all to-do with their details.
  - Mark to-do as complete.
  - Remove specific to-do with or without confirmation.
  - Clear all to-do from the database.
- **Help Documentation**: Easily accessible help options for all commands.

---

## Installation

1. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Run the application:
   ```bash
   python3 -m rptodo --help
   ```


---
## Commands

| Command | Description |
|---------|-------------|
| `python3 -m rptodo --help` | Show details about the to-do CLI application. |
| `python3 -m rptodo --version` | Display the version of the application. |
| `python3 -m rptodo init` | Initialize the to-do app with a database. |
| `python3 -m rptodo list` | List all to-do items. |
| `python3 -m rptodo add "<task>" -p <priority>` | Add a task with an optional priority (default: 2). |
| `python3 -m rptodo complete <id>` | Mark a task as completed using its ID. |
| `python3 -m rptodo remove <id>` | Remove a task by ID (requires confirmation). |
| `python3 -m rptodo remove <id> --force` | Remove a task by ID without confirmation. |
| `python3 -m rptodo clear` | Remove all tasks from the database (requires confirmation). |

### Examples

1. **Add a task**:
   ```bash
   python3 -m rptodo add "Buy groceries" -p 2
   ```

2. **List all tasks**:
   ```bash
   python3 -m rptodo list
   ```

3. **Mark a task as completed**:
   ```bash
   python3 -m rptodo complete 1
   ```

4. **Remove a task with confirmation**:
   ```bash
   python3 -m rptodo remove 1
   ```
5. **Remove a task without confirmation**:
   ```bash
   python3 -m rptodo remove 1 --force
   ```

6. **Clear all tasks from the database**:
   ```bash
   python3 -m rptodo clear
   ```

   
---
## Usage

### Getting Started

1. **Initialize the app**:
   ```bash
   python3 -m rptodo init
   ```
   This sets up the database to store your tasks.

2. **View available commands**:
   ```bash
   python3 -m rptodo --help
   ```

3. **Add your first task**:
   ```bash
   python3 -m rptodo add "Complete Real Python course" -p 1
   ```




---