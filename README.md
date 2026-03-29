# Bank Management System - SOLID & Design Patterns

A comprehensive Java-based banking system redesigned with a focus on **Software Architecture**, **SOLID Principles**, and **Design Patterns** to ensure scalability, maintainability, and clean code practices.

## 🚀 Key Architectural Improvements

### 🏗️ SOLID Principles Implementation
* **Single Responsibility:** Decoupled business logic, data management, and user interaction into specialized modules.
* **Open/Closed:** The system is easily extendable for new account types (e.g., Investment accounts) without modifying existing core logic.
* **Interface Segregation:** Used specific interfaces like `Profitable`, `Vipable`, and `ManagementFees` to ensure classes only implement necessary methods.

### 🧩 Design Patterns Applied

* **Facade Pattern:** Simplified system complexity by implementing dedicated Facades:
    * `AccountFacade`: Manages account lifecycle and client operations.
    * `ReportFacade`: Handles statistics and data visualization.
    * `CalculationFacade`: Centralizes financial algorithms and profit calculations.
* **Observer Pattern:** Integrated a real-time notification system. The `BankObserver` (Subject) triggers updates to multiple observers (`Action1`, `Action2`) upon critical system events.
* **Singleton Pattern:** The `Bank` class is implemented as a thread-safe Singleton to ensure global access and data consistency across the application.
* **Factory Pattern:** Centralized object instantiation through `AccountsFactory`, allowing for dynamic creation of diverse account types (Checking, Savings, Mortgage) while maintaining loose coupling.
* **Iterator & ListIterator:** Developed custom `CustomIterator` and `CustomListIterator` implementations for safe, encapsulated traversal of financial data collections.

## 🛠️ Technical Stack & Features
* **Language:** Java (JDK 11+)
* **Data Integrity:** Custom Exception Handling for financial transaction safety.
* **Generics & Collections:** Advanced use of Java Collections and Generics for type-safe data structures.
* **Automation:** Built-in automated data generation for system testing and demonstration.

## 📂 Project Structure
```text
src/
├── main/                 # Core logic, Facades, and Models
├── interfaces/           # Abstractions and Segregated Interfaces
├── bankManagement/       # Observer logic and Bank Singleton
├── bankException/        # Custom business logic exceptions
└── bankEnum/             # System-wide constants and types
