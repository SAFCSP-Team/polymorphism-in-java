# Polymorphism Project

### Objective

The project’s main goal is to understand how polymorphism works in Java via **method overriding**, **method overloading**, and using **parent references**. 

### Problem

Create a Java program with a parent class `Employee` and child classes `FullTimeEmployee` and `PartTimeEmployee` to demonstrate method overriding and overloading. Use a parent reference to manage all employee instances in the main method.

### Implementation

- Create a parent class `Employee` with:
  - A `String name`.
  - A constructor for the name.
  - A `double calculateSalary()` method that returns 0.

- Create a **`FullTimeEmployee`** subclass:
    - Add a `double monthlySalary`.
    - Override `calculateSalary()` to return the monthly salary.
    - An **overloaded** `calculateSalary(double bonus)` method that returns the bonus + monthly salary.

- Create a **`PartTimeEmployee`** subclass:
    - Add properties `double hourlyRate` and `int hoursWorked`,
    - Override `calculateSalary()` to return `hourlyRate * hoursWorked`.

- In the `main` method:
  - Create objects from the `FullTimeEmployee` and `PartTimeEmployee`, both using the parent.
  - Use the parent reference to print each employee’s name and calculated salary by calling their methods.
  - Call the overloaded method with a bonus.

