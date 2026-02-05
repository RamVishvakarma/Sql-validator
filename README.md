# SQL Validator Console Application

## Overview

The **SQL Validator Console Application** is a lightweight, console-based tool designed to **validate SQL queries without executing them**.  
It performs **static analysis** to detect syntax, structural, and rule-based errors in SQL statements and provides clear, human-readable feedback.

The project is built with a **modular and extensible architecture**, making it suitable for learning, training programs, and future enhancements such as dialect support or advanced validation rules.

---

## Why This Project Exists

SQL errors are often detected **only at runtime** after queries are sent to a database.  
This project aims to **shift error detection earlier** in the development process by validating queries before execution.

It is especially useful for:
- Learning and practicing SQL
- Validating queries during development
- Code reviews and quality checks
- Training and educational environments

---

## Key Features

- Console-based interactive validation
- Supports both **DML and DDL** SQL statements
- Handles **single-line and multi-line queries**
- Detects multiple errors in a single validation run
- Clear and structured error reporting
- Modular validation engine for easy extensibility
- No database connection required
- Uses only Python standard libraries

---

## Validation Scope

The validator focuses on **syntax and structural correctness**, including:
- Keyword and clause ordering
- Required clause presence
- Parenthesis and quote balancing
- Basic expression and operator validation
- Detection of malformed SQL constructs

> ⚠️ This tool **does not execute SQL** and does not validate data against a database schema.

---

## Design Philosophy

- **Separation of concerns**  
  Each component has a single responsibility (input handling, parsing, validation, error reporting).

- **Extensibility**  
  New validation rules or SQL dialects can be added without changing core logic.

- **Reliability**  
  Invalid or malformed input is handled gracefully without crashes.

- **Clarity**  
  Errors are reported in a simple, understandable format suitable for beginners and professionals alike.

---

## Intended Audience

- Students and learners of SQL
- Software engineers
- Database developers
- QA engineers
- Training and onboarding programs

---

## Project Status

This project is part of a **company training program** and focuses on:
- Clean design
- Proper documentation
- Logical architecture
- Maintainable code structure

Future enhancements are planned as part of continued learning and improvement.

---

## License

This project is intended for **educational and training purposes**.
