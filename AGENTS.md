# AGENTS.md - AI Coding Agent Guidelines

These guidelines outline the principles and requirements for the development of AI coding agents within this repository. Adherence to these principles is crucial for maintaining a sustainable, well-structured, and easily maintainable codebase.

## 1. DRY (Don't Repeat Yourself)

*   **Single Responsibility Principle:** Each agent should have a single, clearly defined purpose. Avoid creating redundant code for similar functionalities.
*   **Module Decomposition:** Break down complex tasks into smaller, reusable modules. Each module should have a well-defined interface and minimal dependencies.
*   **Abstraction:** Define abstract interfaces for agents and their functionalities. This allows for flexibility and easier modification without affecting core agent logic.

## 2. KISS (Keep It Simple, Stupid)

*   **Minimal Code:** Strive for the shortest possible code that achieves the desired functionality. Avoid unnecessary complexity.
*   **Readability:** Prioritize code that is easy to understand and maintain. Use clear naming conventions and comments where necessary.
*   **Algorithm Efficiency:** Ensure algorithms are computationally efficient and avoid unnecessary iterations or calculations.

## 3. SOLID Principles

*   **Single Responsibility:** Each class/agent should have a single reason to change.
*   **Open/Closed Principle:**  The system should be extensible through mechanisms like interfaces and abstract classes, without modifying the core implementation.
*   **Liskov Substitution Principle:**  Subclasses should be substitutable for their base classes without altering the correctness of the program.
*   **Interface Segregation Principle:** Client code should not be required to depend on implementation details of the interface they are using.
*   **Dependency Inversion Principle:** High-level modules should not depend on low-level modules; they should depend on abstractions.

## 4. YAGNI (You Aren't Gonna Need It)

*   **Future-Proofing:**  Don't introduce functionalities that are likely to be obsolete or require future modifications.
*   **Focus on Current Requirements:**  Prioritize the implementation of necessary features based on the current task requirements.
*   **Refactoring:**  Avoid unnecessary refactoring that adds complexity.  Refactor only when the existing code is not sufficiently complex.

## 5. Code Constraints

*   **Maximum Code Length:** 180 lines of code per file.
*   **Test Coverage Minimum:** 80% minimum.  All files must contain a substantial amount of test code.

## 6. Development Process

*   **Code Reviews:**  Mandatory code reviews for all significant changes.
*   **Unit Testing:** Comprehensive unit tests for each module.
*   **Integration Testing:**  Testing of the interaction between agent modules.
*   **Static Analysis:** Utilize static analysis tools (e.g., pylint, flake8) to detect potential errors and code style violations.
*   **Version Control:** Use Git for version control.
*   **Documentation:** Maintain clear and concise documentation for all agents and modules.

## 7.  Testing Frameworks

*   Utilize a testing framework (e.g., pytest) for automated testing.
*   Create test suites that cover all critical functionalities.

## 8. Data Handling

*   All data should be handled as data, not as values.  Avoid direct manipulation of data within code.
*   Utilize external data sources where appropriate, and document the data flow clearly.

## 9.  API Design (Agent Interface)

*   Define clear and well-documented APIs for all agent functionalities.
*   Employ structured data formats (e.g., JSON) for data exchange.
*   Ensure APIs are robust and handle potential errors gracefully.

## 10.  File Structure (Example)

```
agents.md
├── __init__.py
├── agent_a.py
├── agent_b.py
├── modules/
│   ├── data_processing.py
│   ├── logic_engine.py
│   └── utils.py
└── tests/
    ├── __init__.py
    ├── test_agent_a.py
    ├── test_agent_b.py
    └── ...
```

These guidelines are a living document and should be reviewed and updated periodically.  Any deviation from these guidelines must be thoroughly justified and documented.