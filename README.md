# Car Showroom Management System

## Overview

The Car Showroom Management System is a Java-based application designed to manage showrooms, employees, and cars efficiently. This system leverages Object-Oriented Programming (OOP) principles to provide a robust, modular, and easy-to-maintain codebase.

## Features

- **Add Showrooms**: Input details for new showrooms.
- **Add Employees**: Input details for new employees and assign them to showrooms.
- **Add Cars**: Input details for new cars and associate them with showrooms.
- **View Showrooms**: Retrieve and display details of all showrooms.
- **View Employees**: Retrieve and display details of all employees.
- **View Cars**: Retrieve and display details of all cars.

## Technologies Used

- **Programming Language**: Java
- **Development Paradigm**: Object-Oriented Programming (OOP)

## Classes and Interfaces

### Interface `Utility`

This interface defines the methods that must be implemented by any class that implements it. It contains two methods:

- `void get_details()`
- `void set_details()`

### Class `Showroom`

Implements the `Utility` interface to manage showroom details.

Attributes:
- `String showroom_name`
- `String showroom_address`
- `int total_employees`
- `int total_cars_in_stock`
- `String manager_name`

Methods:
- `void get_details()`
- `void set_details()`

### Class `Employees`

Extends the `Showroom` class to include employee-specific details.

Attributes:
- `String emp_id`
- `String emp_name`
- `int emp_age`
- `String emp_department`

Methods:
- `void get_details()`
- `void set_details()`

### Class `Cars`

Extends the `Showroom` class to include car-specific details.

Attributes:
- `String car_name`
- `String car_color`
- `String car_fuel_type`
- `int car_price`
- `String car_type`
- `String car_transmission`

Methods:
- `void get_details()`
- `void set_details()`

## Main Application Class `App`

The `App` class contains the main method and handles the user interaction, including displaying the main menu and processing user inputs.

### Main Menu

Displays options for the user:
- Add Showrooms
- Add Employees
- Add Cars
- Get Showrooms
- Get Employees
- Get Cars
- Exit

### Main Method

Handles the main loop and user input processing:
- Initializes arrays to store instances of `Showroom`, `Employees`, and `Cars`.
- Uses a `Scanner` to read user input.
- Provides a switch-case structure to handle different user choices.

## How to Run

1. Compile the Java files:
   ```sh
   javac App.java
