# Astronaut Daily Schedule Organizer

This is a console-based application that helps astronauts organize their daily schedules.  
It has been designed with a focus on clean code, adherence to SOLID principles, and the use of design patterns (Singleton, Factory, Observer).  
The project evaluates skills in OOP, exception handling, logging, and maintainable code structure.

---

## Problem Statement

The application allows astronauts to manage their daily tasks. Each task has:
- Title
- Description
- Start time
- End time
- Priority level (High, Medium, Low)

The program ensures that tasks do not overlap, validates user input, and provides clear error messages. It is a simple CLI application that focuses on logic and code quality rather than UI.

---

## Features

### Mandatory
1. Add a new task with title, description, start time, end time, and priority level.
2. Remove an existing task.
3. View all tasks sorted by start time.
4. Validate that new tasks do not overlap with existing tasks.
5. Provide appropriate error messages for invalid operations.

### Optional (Partially Implemented / Extensible)
1. Mark tasks as completed.
2. View tasks filtered by priority.
3. Extendable to support editing of tasks.

---

## Design Patterns Used

1. **Singleton Pattern**
   - Implemented in `ScheduleManager`.
   - Ensures only one instance of the schedule manager exists.

2. **Factory Pattern**
   - Implemented in `TaskFactory`.
   - Responsible for creating tasks with validation for time format and priority.

3. **Observer Pattern**
   - Implemented via `Observer` and `ConsoleObserver`.
   - Observers are notified when conflicts occur or updates happen.
   - Console output and logging are used to provide notifications.

---



