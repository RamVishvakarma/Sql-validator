# SQL Validator – Requirements Document

---

## Project Name
**SQL Validator Console Application**

A console-based system for validating SQL queries for syntax, structure, and standard compliance without executing them.

---

## Table of Contents

1. Overview  
2. Functional Requirements  
3. Non-Functional Requirements  
4. System Scope  
5. Dependencies & Constraints  
6. Success Criteria  
7. Out of Scope  
8. Future Enhancements  

---

## 1. Overview

### 1.1 Purpose
The purpose of this project is to design and implement a modular SQL validation engine that checks SQL queries for correctness, structure, and rule compliance using static analysis.

### 1.2 Target Users
- Software Engineers
- Database Developers
- Students & Trainees
- QA Engineers
- DevOps Teams (CI validation)

### 1.3 Use Cases
- Validate SQL queries before execution
- Learn correct SQL syntax
- Detect errors early in development
- Review SQL during code reviews
- Batch validation of SQL files

---

## 2. Functional Requirements

### 2.1 SQL Query Input
The system shall accept SQL queries via a console interface.

**Acceptance Criteria**
- Accept single-line queries
- Accept multi-line queries
- Accept nested queries
- Accept batch input
- Support interactive mode

---

### 2.2 Supported SQL Statements

**DML Statements**
- SELECT
- INSERT
- UPDATE
- DELETE

**DDL Statements**
- CREATE
- ALTER
- DROP
- TRUNCATE

---

### 2.3 Query Validation
The system shall validate SQL queries without executing them.

**Validation Scope**
- Syntax correctness
- Required clause presence
- Clause ordering
- Parenthesis matching
- Quote matching
- Operator validation

---

### 2.4 Error Detection & Reporting
The system shall report all detected errors.

**Acceptance Criteria**
- Detect multiple errors in a single query
- Display clear error messages
- Indicate error type
- Indicate error location (line-based if possible)
- Categorize errors (syntax / structure)

---

### 2.5 Interactive Mode
The system shall support interactive validation.

**Acceptance Criteria**
- Accept repeated user input
- Validate immediately
- Allow graceful exit
- Display validation result clearly

---

### 2.6 Extensibility
The system shall support future extensions.

**Acceptance Criteria**
- Add new SQL rules without core changes
- Add new validation strategies
- Support additional SQL dialects

---

## 3. Non-Functional Requirements

### 3.1 Performance
- Single query validation < 100 ms
- Batch processing supported
- Linear time complexity O(n)

---

### 3.2 Reliability
- No crashes on invalid input
- Graceful error handling
- Consistent validation output

---

### 3.3 Maintainability
- Modular architecture
- Clear separation of concerns
- Well-documented logic

---

### 3.4 Portability
- Cross-platform (Windows, Linux, macOS)
- Python 3.8+

---

### 3.5 Security
- No SQL execution
- Safe handling of user input
- No external system interaction

---

## 4. System Scope

### In Scope
- SQL syntax validation
- Console-based interaction
- Rule-based validation engine

### Out of Scope
- Database connectivity
- Query execution
- Query optimization

---

## 5. Dependencies & Constraints
- Python standard library only
- No third-party SQL parsers
- Offline execution

---

## 6. Success Criteria
The project is successful if:
1. All supported SQL statements are validated correctly
2. Errors are reported clearly
3. Architecture supports extension
4. Application runs without crashes
5. Documentation is complete

---

## 7. Out of Scope
- SQL execution
- Performance benchmarking
- Web interface
- Schema validation

---

## 8. Future Enhancements
- Support for more SQL dialects
- IDE integration
- Query formatting
- Semantic validation
