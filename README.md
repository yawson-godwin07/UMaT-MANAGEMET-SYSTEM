# UMaT Management System (Inheritance Practice)

This repository contains a simple Python implementation of a campus management system for the University of Mines and Technology (UMaT). The project demonstrates the core Object-Oriented Programming (OOP) concept of **inheritance** by managing different roles on campus.

## Task Overview

The goal is to design a system that handles common information shared by all individuals on campus (like name and age) while allowing specific roles—such as **Students** and **Lecturers**—to have their own unique attributes and responsibilities.

### Requirements Implemented:
1. **Base Class (`Person`):** Houses shared attributes (`name`, `age`) and a base `display_info()` method.
2. **Derived Classes (`Student` & `Lecturer`):** * `Student` adds a `student_id` and an `enroll_course()` method.
   * `Lecturer` adds an `employee_id` and a `teach_course()` method.
3. **Super Function (`super()`):** Used to initialize inherited attributes from the parent class cleanly.
4. **Method Overriding:** The `Student` class overrides `display_info()` to include its unique ID while leveraging `super().display_info()` to print the basic details.

---

## Code Structure

* **`Person`**: The parent class.
* **`Student(Person)`**: Inherits from Person; handles student-specific data.
* **`Lecturer(Person)`**: Inherits from Person; handles lecturer-specific data.

---

## How to Run the Script

Ensure you have Python installed on your machine. Clone the repository and run the script using your terminal or an IDE:

```bash
pythonumat_management.py
--- Testing Student ---
Name: Godwin
Age: 19
Student ID: UMaT-ST-01
Godwin has enrolled in Introduction to Python.

--- Testing Lecturer ---
Name: Mr. Cobbinah
Age: 40
Mr. Cobbinah is teaching Object-Oriented Programming.
