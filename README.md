# Task & Habit Manager

A simple command‑line Task and Habit Tracker implemented in Python. This script lets you add, complete, remove, and report on your daily tasks and recurring habits through a clean, interactive menu interface.

## Features

* **Add** new tasks or habits interactively
* **Mark** tasks or habits as complete
* **Remove** existing tasks or habits
* **View Reports**

  * **Daily Report**: Shows all tasks/habits for a specific day and their statuses
  * **Weekly Report**: Summarizes completion counts for each habit and lists completed/incomplete tasks over the week
* **Random Motivational Quotes** displayed on each menu refresh
* **Cross‑platform console clearing** for a clean UI (Windows & Unix)

## Prerequisites

* Python 3.6 or newer

## Installation

1. Clone or download this repository to your local machine:

   ```bash
   git clone <repository_url>
   cd <project_folder>
   ```
2. (Optional) Create a virtual environment:

   ```bash
   python3 -m venv venv
   source venv/bin/activate    # Unix/macOS
   venv\Scripts\activate     # Windows
   ```
3. Install any dependencies (none required beyond the standard library):

   ```bash
   pip install --upgrade pip
   ```

## Usage

Run the script from your terminal:

```bash
python task_habit_manager.py
```

Follow the on‑screen prompts:

1. **Add a Task or Habit**: Enter `T` or `Task` / `H` or `Habit`
2. **Complete a Task or Habit**: Choose which to mark done
3. **Remove a Task or Habit**: Delete entries you no longer need
4. **View Reports**: Select `Daily` or `Weekly` to see progress summaries
5. **Exit**: Quit the program

## Code Organization

* `clear_console()`: Clears the terminal window for both Windows (`cls`) and Unix (`clear`).
* `display()`: Prints a header banner and a random motivational quote.
* `get_menu_choice()`: Presents the main menu and returns the user’s selection.
* `add_task()`, `add_habit()`: Prompt for and store new tasks/habits.
* `task_comp()`, `habit_comp()`: Mark existing items as complete for a given day.
* `rem_task()`, `rem_habit()`: Remove tasks/habits from the tracker.
* `day_report()`: Shows all entries and their statuses for a specified day.
* `week_report()`: Summarizes habit completion counts and task status lists for the week.
* `main()`: Orchestrates the loop: display → input → action → repeat.



