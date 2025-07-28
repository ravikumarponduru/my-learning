# 📘 Java Beginner’s Learning Guide

This guide offers a detailed roadmap for mastering **Core Java** as a beginner. It covers essential syntax, concepts, examples, and best practices to build a solid foundation for further Java development.

---

## ✅ 1. Introduction to Java

### 🔹 What is Java?
Java is a **high-level**, **object-oriented**, **class-based**, and **platform-independent** programming language.

- **WORA (Write Once, Run Anywhere)** – Java programs run on the JVM, which makes them platform-independent.
- Java is widely used for building:
  - Desktop applications
  - Web applications
  - Mobile apps (Android)
  - Embedded systems
  - Enterprise-grade back-end services

### 🔹 Key Features of Java
- **Simple**: Easy syntax, similar to C++
- **Object-Oriented**: Everything is part of a class
- **Platform Independent**: Runs on any OS with JVM
- **Robust**: Strong memory management
- **Secure**: Bytecode verification, exception handling
- **Multithreaded**: Supports parallel execution
- **Portable**: Bytecode is architecture-neutral

---

## ✅ 2. Java Syntax, Variables, and Data Types

### 🔹 Basic Syntax
- Java code is **case-sensitive**
- Classes and methods must be **within a class**
- Every application starts with the `main()` method

### 🔹 Variables and Data Types

```java
int age = 25;
double price = 99.99;
char grade = 'A';
boolean isLoggedIn = true;
String name = "Alice";
```

| Type      | Example                | Description                   |
|-----------|------------------------|-------------------------------|
| `int`     | `int count = 100;`     | Whole numbers                 |
| `double`  | `double rate = 9.99;`  | Decimal numbers               |
| `char`    | `char c = 'A';`        | Single 16-bit Unicode char    |
| `boolean` | `boolean b = false;`   | true or false                 |
| `String`  | `String msg = "Hi";`   | Sequence of characters        |

---

## ✅ 3. Operators and Conditionals

### 🔹 Arithmetic Operators

```java
int a = 10;
int b = 3;
System.out.println(a + b);  // 13
System.out.println(a / b);  // 3
```

### 🔹 Comparison Operators

```java
a == b  // equal
a != b  // not equal
a > b   // greater than
a <= b  // less than or equal
```

### 🔹 Logical Operators

```java
(a > 5) && (b < 10)
(a == 5) || (b == 3)
!(a > b)
```

### 🔹 Conditional Statements

```java
int score = 85;

if (score >= 90) {
    System.out.println("Excellent!");
} else if (score >= 70) {
    System.out.println("Good job!");
} else {
    System.out.println("Needs improvement.");
}
```

### 🔹 Switch Statement

```java
int day = 2;

switch (day) {
    case 1:
        System.out.println("Monday");
        break;
    case 2:
        System.out.println("Tuesday");
        break;
    default:
        System.out.println("Another day");
}
```

---

## ✅ 4. Loops in Java

### 🔹 `for` Loop

```java
for (int i = 0; i < 5; i++) {
    System.out.println("i = " + i);
}
```

### 🔹 `while` Loop

```java
int i = 0;
while (i < 5) {
    System.out.println(i);
    i++;
}
```

### 🔹 `do-while` Loop

```java
int i = 0;
do {
    System.out.println(i);
    i++;
} while (i < 5);
```

### 🔹 Enhanced `for-each` Loop

```java
int[] numbers = {1, 2, 3, 4};
for (int num : numbers) {
    System.out.println(num);
}
```

---

## ✅ 5. Methods (Functions)

### 🔹 Defining and Calling Methods

```java
public class Calculator {
    public static int add(int a, int b) {
        return a + b;
    }

    public static void main(String[] args) {
        int result = add(5, 3);
        System.out.println("Sum: " + result);
    }
}
```

### 🔹 Method Overloading

```java
void greet() {
    System.out.println("Hello!");
}

void greet(String name) {
    System.out.println("Hello, " + name);
}
```

---

## ✅ 6. Arrays

### 🔹 Declare and Initialize Arrays

```java
int[] scores = {90, 85, 78};
String[] names = new String[3];
```

### 🔹 Access Elements

```java
System.out.println(scores[0]); // 90
```

### 🔹 Loop Through Array

```java
for (int i = 0; i < scores.length; i++) {
    System.out.println(scores[i]);
}
```

---

## ✅ 7. Object-Oriented Programming (OOP)

### 🔹 Class & Object

```java
class Car {
    String color;

    void drive() {
        System.out.println("Car is driving");
    }
}

public class Main {
    public static void main(String[] args) {
        Car myCar = new Car();
        myCar.color = "Red";
        myCar.drive();
    }
}
```

### 🔹 Constructors

```java
class Car {
    String model;

    Car(String m) {
        model = m;
    }
}
```

### 🔹 `this` Keyword

```java
class Student {
    String name;

    Student(String name) {
        this.name = name;
    }
}
```

### 🔹 Static Members

```java
class MathUtil {
    static int add(int a, int b) {
        return a + b;
    }
}
```

---

## ✅ 8. 4 Pillars of OOP

### 🔹 Encapsulation

```java
class Person {
    private String name;

    public String getName() {
        return name;
    }

    public void setName(String n) {
        name = n;
    }
}
```

### 🔹 Inheritance

```java
class Animal {
    void sound() {
        System.out.println("Animal sound");
    }
}

class Dog extends Animal {
    void bark() {
        System.out.println("Dog barks");
    }
}
```

### 🔹 Polymorphism

#### Method Overriding
```java
class Animal {
    void sound() {
        System.out.println("Animal sound");
    }
}

class Cat extends Animal {
    @Override
    void sound() {
        System.out.println("Meow");
    }
}
```

#### Method Overloading
```java
int add(int a, int b) { return a + b; }
double add(double a, double b) { return a + b; }
```

### 🔹 Abstraction

#### Using Abstract Class
```java
abstract class Shape {
    abstract void draw();
}

class Circle extends Shape {
    void draw() {
        System.out.println("Drawing Circle");
    }
}
```

#### Using Interface
```java
interface Vehicle {
    void start();
}

class Car implements Vehicle {
    public void start() {
        System.out.println("Car started");
    }
}
```

---

## ✅ 9. Access Modifiers

| Modifier     | Scope                                 |
|--------------|----------------------------------------|
| `public`     | Everywhere                            |
| `private`    | Inside the same class only            |
| `protected`  | Same package + subclasses             |
| *no modifier*| Package-private (default)             |

---

## ✅ 10. Constants (`final`)

```java
final double PI = 3.14159;
```

- `final` variables cannot be changed after initialization
- Convention: Use ALL_CAPS for constant names

---

## ✅ 11. Packages and Imports

### 🔹 Packages

```java
package com.example.myapp;
```

Save the file under `/com/example/myapp/`

### 🔹 Imports

```java
import java.util.Scanner;
import java.util.ArrayList;
```

---

## ✅ 12. Exception Handling

```java
try {
    int result = 10 / 0;
} catch (ArithmeticException e) {
    System.out.println("Error: " + e.getMessage());
} finally {
    System.out.println("Cleanup done.");
}
```

---

## ✅ 13. Java Utility Classes (Intro)

### 🔹 Scanner (Input)

```java
import java.util.Scanner;

Scanner sc = new Scanner(System.in);
System.out.print("Enter name: ");
String name = sc.nextLine();
```

### 🔹 Math

```java
int max = Math.max(10, 20);
double sqrt = Math.sqrt(25);
```

### 🔹 ArrayList

```java
import java.util.ArrayList;

ArrayList<String> list = new ArrayList<>();
list.add("Java");
list.add("Python");
```

---

## ✅ 14. Summary Table

| Concept        | Description                         |
|----------------|-------------------------------------|
| Variables      | Store data                          |
| Data Types     | Define type of data                 |
| Operators      | Perform calculations and logic      |
| Conditionals   | `if`, `else`, `switch`              |
| Loops          | `for`, `while`, `do-while`          |
| Methods        | Reusable blocks of code             |
| Classes        | Blueprint for objects               |
| Objects        | Instance of a class                 |
| OOP            | Inheritance, Polymorphism, etc.     |
| Exception      | Handle runtime errors               |
| Packages       | Organize code into namespaces       |
| Imports        | Use built-in or custom packages     |

---

## ✅ 15. Exercises

- [001](./exercises/001.md)

---

Happy Learning! ☕🚀
