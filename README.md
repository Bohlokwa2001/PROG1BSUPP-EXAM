README Document
Hospital Operations Management System
Module Name: Programming 1B
Course Code: DISD
Student Name: Bohlokwa Letsoso
Student Number: ST10096006
1. Introduction

This document provides an overview of the Hospital Operations Management System developed as part of the Programming 1B (DISD) module. The project consists of two Java-based applications designed to analyse, process, and report operational data for a private hospital.

The assignment is divided into two components:

A console application (Question 1) that processes quarterly operation data and provides statistical outputs.

A graphical user interface (GUI) application (Question 2) that processes surgical operation data and allows the user to generate and save reports.

Both applications make use of interfaces, classes, arrays, Swing components, and unit testing to ensure correctness and modularity.

2. Objectives

The primary objectives of this project are:

To apply object-oriented programming principles using Java.

To implement logic using single-dimensional and two-dimensional arrays.

To demonstrate the use of interfaces to enforce consistent method structures.

To create user-friendly output through a console menu and GUI interface.

To validate functionality using JUnit 5 unit tests.

To perform file handling operations to store processed data.

3. Project Structure
hospital_operations_project/
│
├── Q1/                       # Console Application (Question 1)
│   ├── src/hospital/operations/
│   │   ├── IOperations.java
│   │   ├── Operations.java
│   │   └── Main.java
│   └── tests/hospital/operations/
│       └── OperationsTest.java
│
├── Q2/                       # GUI Application (Question 2)
│   ├── src/hospital/gui/
│   │   ├── IOperationsGUI.java
│   │   ├── OperationsGUI.java
│   │   └── MainGUI.java
│   └── tests/hospital/gui/
│       └── OperationsGUITest.java
│
└── README.md


This structure ensures clear separation between question components and supports maintainability and efficient navigation.

4. Question 1: Console Application
4.1 Description

The console application processes quarterly hospital operation data for two years. Using a two-dimensional array, the system performs the following:

Calculates total operations

Computes average operations

Determines maximum operations

Determines minimum operations

These functionalities are defined in an interface (IOperations) and implemented in the Operations class. A text-based menu system allows the user to select which results to display.

4.2 Data Used
Year	Q1	Q2	Q3
1	320	175	380
2	210	125	360
4.3 Compilation Instructions

Compile:

javac -d out $(find Q1/src -name "*.java")


Run:

java -cp out hospital.operations.Main

4.4 Unit Testing

Unit tests validate:

The correctness of the TotalOperations method

The correctness of the AverageOperations method

Testing follows JUnit 5 conventions, ensuring accurate and reliable results.

5. Question 2: GUI Application
5.1 Description

The GUI application provides a visual interface for processing surgical operation data for two years. It supports:

Processing total operations

Viewing total operations for Year 1

Viewing total operations for Year 2

Saving processed output to data.txt

Clearing the text area

Accessing operations through both button controls and menu items

The interface includes a combo box, buttons, menu bar, and a scrollable text area.

5.2 Data Used
Year	Planned	Unplanned	Emergency
1	300	150	700
2	250	200	600
5.3 Compilation Instructions

Compile:

javac -d out $(find Q2/src -name "*.java")


Run:

java -cp out hospital.gui.MainGUI

5.4 Unit Testing

The following JUnit tests verify correct output:

Total operations for Year 1

Total operations for Year 2

This ensures accuracy of the computational logic within OperationsGUI.

6. Technologies and Tools Used

Java SE

Java Swing (GUI development)

JUnit 5 (Unit Testing Framework)

File I/O (Java FileWriter)

Object-Oriented Programming Principles

Arrays (1D and 2D)

7. Conclusion

This project demonstrates the effective application of Java programming concepts, including interface implementation, GUI design, modular class structure, and data processing. The console and GUI applications successfully meet the requirements of the assignment by providing accurate calculations, clear user interaction, and structured reporting mechanisms. The inclusion of comprehensive unit tests ensures reliability and correctness across both systems.
