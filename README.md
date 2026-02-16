# Polymorphism Project

### Objective

The project’s main goal is to understand polymorphism in Java through method overriding, method overloading, and the use of parent references. 
### Problem
Create a Java program with a parent class `Employee` and child classes `FullTimeEmployee` and `PartTimeEmployee` to demonstrate Method overriding, Method overloading
and using parent references to manage all employee instances.

### Implementation
  - **Create a parent class `Employee`**:
    - Add a `String name` property.
    - Add a constructor that initializes `name`.
    - Implement a `double calculateSalary()` method that returns 0.
    - Implement an **overloaded** method `double calculateSalary(double bonus)` that by default returns `calculateSalary()`

- **Create a `FullTimeEmployee`** that inherits from `Employee`:
  - Add a `double monthlySalary` property.
  - Add a constructor to initialize the `name` and `monthlySalary`.
  - **Override** the `calculateSalary()` method to return the monthly salary.
  - **Override** the overloaded `calculateSalary(double bonus)` method to return `monthlySalary + bonus`.

- **Create a `PartTimeEmployee`** that inherits from `Employee`:
  - Add properties `double hourlyRate` and `int hoursWorked`.
  - Add a constructor to initialize `name`, `hourlyRate`, and `hoursWorked`.
  - **Override** the `calculateSalary()` method to return `hourlyRate * hoursWorked`.
  - **Override** the overloaded `calculateSalary(double bonus)` method to return `(hourlyRate * hoursWorked) + bonus`.

- **In the `main` method**:
  - Create `FullTimeEmployee` and `PartTimeEmployee` objects, both using the parent references.
  - For each object, print their name and salary using the `calculateSalary()` and `calculateSalary(double bonus)` methods.
