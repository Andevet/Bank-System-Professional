# Bank-System-SOLID | Advanced Software Architecture

## Overview
This project is an advanced refactoring of the Bank Management System, completed during the **Advanced Object-Oriented Programming** course. The focus was shifted from basic functionality to high-level software engineering, emphasizing **SOLID principles** and **Design Patterns** to create a decoupled and professional architecture.

## Key Engineering Enhancements

### 1. SOLID Implementation
- **Single Responsibility (SRP):** Completely separated system logic by introducing dedicated **Facades**:
    - `AccountFacade`: Manages account lifecycles.
    - `ReportFacade`: Handles complex data queries and statistics.
    - `CalculationFacade`: Responsible for financial algorithms.
- **Dependency Inversion (DIP):** Modules now depend on abstractions rather than concrete implementations.

### 2. Advanced Design Patterns
- **Memento Pattern:** Implemented a robust "Save & Restore" mechanism for the bank's internal collections (`ArrayList`), allowing the system to revert to previous states safely.
- **Observer Pattern:** Integrated a real-time notification system. Specific system events trigger updates to multiple observers (e.g., `Action1`, `Action2`).
- **Iterator & ListIterator:** Developed custom iterators for safe and efficient collection traversal, including reverse-order printing and specialized data manipulation.

### 3. Data Structures & Generics
- Extensive use of **Java Generics** for type-safety.
- Specialized use of `TreeSet` with custom **Comparators** to handle automated sorting and avoid data duplication based on specific business rules.

## Technical Skills Demonstrated
- Advanced Java Development
- Software Architecture & Refactoring
- GoF Design Patterns
- Clean Code Practices (SOLID)