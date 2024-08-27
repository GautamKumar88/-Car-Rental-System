# -Car-Rental-System
Car Rental System Project Report

Introduction
The Car Rental System is a software application designed to manage the rental and return of cars efficiently. It aims to streamline the process for both customers and the rental service provider, ensuring a smooth and user-friendly experience. This report outlines the project objectives, system architecture, key features, implementation details, and future enhancements.
Objectives
The primary objectives of the Car Rental System are:
1.	To automate the car rental process, reducing manual errors and increasing efficiency.
2.	To provide a user-friendly interface for customers to rent and return cars.
3.	To manage and track car availability and rental records systematically.
System Architecture
The system architecture consists of several core components:
1.	Car Class: Represents individual cars with attributes such as car ID, brand, model, base price per day, and availability status.
2.	Customer Class: Represents customers with attributes such as customer ID and name.
3.	Rental Class: Represents the rental transaction, linking a car and a customer with the rental duration.
4.	CarRentalSystem Class: Manages the overall system, including the list of cars, customers, and rentals. It provides methods to add cars and customers, rent and return cars, and display the system menu.
5.	Main Class: Contains the main method to initialize the system and start the menu-driven interface.

Key Features
1. Car Management
•	Add Car: Allows the administrator to add new cars to the system.
•	Car Availability: Tracks the availability of cars, updating their status when rented or returned.
2. Customer Management
•	Add Customer: Automatically generates a customer ID and adds new customers to the system.
3. Rental Process
•	Rent Car: Allows customers to rent available cars by specifying the car ID and rental duration. It calculates the total rental price and confirms the rental.
•	Return Car: Allows customers to return rented cars by specifying the car ID. It updates the car's availability status and removes the rental record.
4. User Interface
•	Menu-Driven Interface: Provides an interactive console-based menu for users to rent and return cars, enhancing user experience.
Implementation Details
The system is implemented in Java, leveraging object-oriented programming principles to ensure modularity and maintainability.
Class Descriptions
Car Class
•	Attributes: carId, brand, model, basePricePerDay, isAvailable
•	Methods: getCarId(), getBrand(), getModel(), calculatePrice(int rentalDays), isAvailable(), rent(), returnCar()

Customer Class
•	Attributes: customerId, name
•	Methods: getCustomerId(), getName()

Rental Class
•	Attributes: car, customer, days
•	Methods: getCar(), getCustomer(), getDays()

CarRentalSystem Class
•	Attributes: cars, customers, rentals
•	Methods: addCar(Car car), addCustomer(Customer customer), rentCar(Car car, Customer customer, int days), returnCar(Car car), menu(), rentCarMenu(Scanner scanner), returnCarMenu(Scanner scanner)

Main Class
•	Method: main(String[] args)





User Interaction Flow
1.	Rent a Car:
•	User selects the "Rent a Car" option.
•	User enters their name.
•	System displays available cars.
•	User selects a car by entering the car ID and rental duration.
•	System calculates the total price and displays rental information for confirmation.
•	If confirmed, the system updates the car's availability and records the rental.
2.	Return a Car:
•	User selects the "Return a Car" option.
•	User enters the car ID of the car to be returned.
•	System updates the car's availability and removes the rental record.
