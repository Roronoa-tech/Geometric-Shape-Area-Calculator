# Geometric-Shape-Area-Calculator
Geometric Shape Area Calculator

A console-based Java application that calculates the area of geometric shapes using Abstraction, Interfaces, and Polymorphism — core Object-Oriented Programming (OOP) concepts.

Project Description

This project demonstrates the design and implementation of a Geometric Shape Area Calculator using the Shape interface. It showcases how different shapes (Circle, Square) can be unified under a common contract, and how polymorphism allows the same method call to produce shape-specific behaviour at runtime.


Features
Calculate area of a Circle using π × radius²
Calculate area of a Square using side × side
Demonstrates interface-based abstraction
Demonstrates runtime polymorphism
Clean, modular, and easily extensible design — new shapes can be added without modifying existing code



OOP Concepts Used

ConceptHow it's AppliedAbstractionShape interface defines calculateArea() contractImplementationCircle and Square implement the Shape interfacePolymorphismInterface references (Shape s = new Circle(...)) call shape-specific logic at runtimeEncapsulationEach shape class holds its own attributes (radius, side)

GeometricShapeAreaCalc.java
│
├── interface Shape
│   └── calculateArea()          → abstract method contract
│
├── class Circle implements Shape
│   ├── double radius
│   ├── Circle(double radius)    → constructor
│   └── calculateArea()          → returns π × radius²
│
├── class Square implements Shape
│   ├── double side
│   ├── Square(double side)      → constructor
│   └── calculateArea()          → returns side × side
│
└── class Main
    └── main(...)                → creates shape objects and displays areas

    Requirements


Java JDK 8 or above
Any IDE or text editor (VS Code, Eclipse, IntelliJ IDEA, Edit Plus, etc.)



How to Run

1. Compile

bashjavac GeometricShapeAreaCalc.java

2. Run

bashjava Main


Sample Output

Area of Circle with radius 5.0 : 78.53981633974483
Area of Square with side 4.0   : 16.0


Limitations


Only Circle and Square shapes are implemented
Console-based interface only
No user input at runtime (values are hardcoded in main)



Future Enhancements


Add more shapes: Rectangle, Triangle, Trapezoid
Accept user input for shape dimensions at runtime
Add a perimeter calculation method to the Shape interface
GUI implementation using JavaFX or Swing
Export results to a file



References


Herbert Schildt, Java: The Complete Reference, 11th Edition, McGraw-Hill, 2018.
Oracle Java Documentation: https://docs.oracle.com
