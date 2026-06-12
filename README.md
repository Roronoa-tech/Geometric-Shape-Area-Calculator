
# Geometric Shape Area Calculator

A console-based Java application that calculates the area of geometric shapes using **Abstraction**, **Interfaces**, and **Polymorphism** — core Object-Oriented Programming (OOP) concepts.

---

## Developer Information

- **Name:** Aditya Savita
- **Class:** BCA 2A
- **Course:** Object Oriented Programming With Java (RU-100-01-00012)
- **University:** Rungta International Skills University, Bhilai, CG
- **Guide:** Dr. Harsh Multani

---

## Project Description

This project demonstrates the design and implementation of a Geometric Shape Area Calculator using the `Shape` interface. It showcases how different shapes (Circle, Square, Rectangle, and Triangle) can be unified under a common contract, and how polymorphism allows the same method call to produce shape-specific behaviour at runtime.

---

## Features

- Calculate area of a **Circle** using π × radius²
- Calculate area of a **Square** using side × side
- Calculate area of a **Rectangle** using length × breadth
- Calculate area of a **Triangle** using ½ × base × height
- Accepts user input at runtime via **Scanner**
- Demonstrates **interface-based abstraction**
- Demonstrates **runtime polymorphism**
- Clean, modular, and easily extensible design

---

## OOP Concepts Used

| Concept | How it's Applied |
|---|---|
| Abstraction | `Shape` interface defines `calculateArea()` contract |
| Implementation | `Circle`, `Square`, `Rectangle`, and `Triangle` implement the `Shape` interface |
| Polymorphism | Interface references (`Shape s = new Circle(...)`) call shape-specific logic at runtime |
| Encapsulation | Each shape class holds its own attributes (`radius`, `side`, `length`/`breadth`, `base`/`height`) |

---

## Project Structure

```
GeometricShapeAreaCalc.java
│
├── interface Shape
│   └── calculateArea()              → abstract method contract
│
├── class Circle implements Shape
│   ├── double radius
│   ├── Circle(double radius)        → constructor
│   └── calculateArea()              → returns π × radius²
│
├── class Square implements Shape
│   ├── double side
│   ├── Square(double side)          → constructor
│   └── calculateArea()              → returns side × side
│
├── class Rectangle implements Shape
│   ├── double length, breadth
│   ├── Rectangle(double l, double b) → constructor
│   └── calculateArea()              → returns length × breadth
│
├── class Triangle implements Shape
│   ├── double base, height
│   ├── Triangle(double b, double h) → constructor
│   └── calculateArea()              → returns ½ × base × height
│
└── class Main
    └── main(...)                    → takes user input via Scanner, creates shape objects and displays areas
```

---

## Requirements

- Java JDK 8 or above
- Any IDE or text editor (VS Code, Eclipse, IntelliJ IDEA, Edit Plus, etc.)

---

## How to Run

### 1. Compile

```bash
javac GeometricShapeAreaCalc.java
```

### 2. Run

```bash
java Main
```

---

## Sample Output

```
Enter radius of Circle: 5
Area of Circle : 78.53981633974483

Enter side of Square: 4
Area of Square : 16.0

Enter length and breadth of Rectangle: 6 3
Area of Rectangle : 18.0

Enter base and height of Triangle: 5 8
Area of Triangle : 20.0
```

---

## References

- Herbert Schildt, *Java: The Complete Reference*, 11th Edition, McGraw-Hill, 2018.
- Oracle Java Documentation: https://docs.oracle.com
