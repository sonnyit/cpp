---
title: Java Basic - Basic Syntax
updated: 2015-12-01
categories:
  - java-basic
tags:
  - java-basic
---

A Java program it can be defined as **a collection of objects** that **communicate** via **invoking** each **other's methods**.

* **Object -** Objects have **states** and **behaviors**.
* **Class -** A class can be defined as a template/blue print that describles the behaviors/states that object of its type support.
* **Methods -** A methods is basically a behavior. A class can contain many methods.
* **Instance Variables -** Each object has its unique set of instance variables. An object's state is create by the values assigned to these instance variables.

### Tables

* [Example First Java Program](#example-first-java-program-10548tables)
* [Basic Syntax](#basic-syntax-10548tables)
* [Java Identifiers](#java-identifiers-10548tables)
* [Java Modifiers](#java-modifiers-10548tables)
* [Java Variables](#java-variables-10548tables)
* [Java Arrays](#java-arrays-10548tables)
* [Java Enums](#java-enums-10548tables)
* [Inheritance](#inheritance-10548tables)
* [Interfaces](#interfaces-10548tables)

## Example First Java Program [&#10548;](#tables)

```java
public class MyFirstJavaProgram {
    /* This is my first java program. 
    * This will print 'Hello World' as the output
    */
    public static void main(String []args) {
    System.out.println("Hello World"); // prints Hello World
    }
} 
```

Put this code in a file's name "MyFirstJavaProgram.java" (must exactly typo). Compile and run with:

```bash
$javac MyFirstJavaProgram.java
$java MyFirstJavaProgram
Hello World
```

## Basic Syntax [&#10548;](#tables)
With Java programs, it is **very important** to keep in mind the following points:

1. **Case Sensitivity -** Java is case sensitive, so **Hello** and **hello** have different meaning in Java.
2. **Class Names -** For all class names, the **first letter** should be in **Upper Case**. Ex: *MyFirstJavaClass*.
3. **Method Names -** All method names should start with a **Lower Case** letter. Ex: *public void myMethodName()*.
4. **Program File Name -** Name of the program file should **exactly match** the (only) **public class name** in this file. Ex: assume 'MyFirstJavaProgram' is the class name. Then the file should be saved as 'MyFirstJavaProgram.java'.
5. **public static void main(String args[]) -** Java program processing starts from the main() methods which is a mandatory part of every Java program.
6. a single line comment **``(//)``**, a multiline comment **``(/* */)``**, and a Javadoc comment **``(/** */)``**.
7. Java code is organized into folders called packages. To reference classes in other packages, you use an **import** statement. A wildcard (**``*``**) ending an import statement means you want to import all classes in that package. It does not include packages that are inside that one. **java.lang** is a special package that does not need to be imported. **Note:** importing by classname takes precedence over wildcards.
8. Constructors create Java objects. A constructor is a method matching the class name and omitting the return type. When an object is instantiated, fields and blocks of code are initialized first. Then the constructor is run.

## Java Identifiers [&#10548;](#tables)
In Java, we have several points that will need to remember about identifiers:

1. All identifiers should begin with a letter **(A-Z or a-z)**, currency character **$** or underscore **_**.
2. After the first character, identifiers can have any combination of character.
3. Identifier **cannot** have the same name with any **keyword**.
4. Most importantly identifiers are case sensitive.
5. Example of **legal** identifiers: age, $salary, _value, __1_value.
6. Example of **illegal** identifiers: 123abc, -salary.

## Java Modifiers [&#10548;](#tables)
Like other languages, it is possible to modify classes, methods, etc., by using modifiers. There are two categories of modifiers:

* **Access Modifiers:** default, public, protected, private.
* **Non-access Modifiers:** final, abstract, strictfp.

## Java Variables [&#10548;](#tables)
Types of variables in Java are:

* Local Variables
* Class Variables (Static Variables)
* Instance Variables (Non-static variables)

Declaring a variable involves stating the data type and giving the variable a name. Variables that represent fields in a class are automatically initialized to their corresponding "zero" or null value during object instantiation. Local variables must be specically initialized. Identifiers may contain letters, numbers, $, or _. Identifiers may not begin with numbers.

## Java Arrays [&#10548;](#tables)
**Arrays** are **objects** that **store** multiple variables of the **same type**. However, an array itself is an object **on the heap**.

## Java Enums
Enums were introduced in Java 5.0. Enums restrict a variable to have **one of only a few predefined values**. The values in this enumerated list are called enums.

**Note:**

* Enums can be declared as **their own** or **inside a class**.
* Methods, variables, constructors can be defined inside enums as well.

## Inheritance [&#10548;](#tables)
In Java, classes can be derived from classes.

This concept allows you to reuse the fields and methods of the existing class without having to rewrite this code in a new class. In this scenario:

* The existing class is called the superclass.
* The derived class is called the subclass.

## Interfaces [&#10548;](#tables)
In Java language, an interface can by defined as a contract between objects on how to communicate with each other. Interfaces play a vital role when it comes to the concept of inheritance.

An interface defines the methods, a deriving class (subclass) should use. But the implementation of the methods is totally up to the subclass.

