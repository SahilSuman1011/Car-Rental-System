# Car Rental System

This Car Rental System is a simple command-line application developed in C++ with MySQL integration. It allows users to view available cars, select one for booking, and update the availability status in real-time.

## Features

- **View Available Cars**: Users can view a list of available cars, including brand, model, serial number, and rental price.
- **Real-time Availability**: The system checks if a car is available for booking, and once booked, the car’s availability status is updated in the database.
- **SQL Integration**: Utilizes MySQL for storing and managing car data (e.g., car serial number, availability, rent, etc.).
- **CRUD Operations**: Supports database operations such as retrieving data, updating availability, and inserting new records for cars.

## Technology Stack

- **C++**: Core programming language used for application logic.
- **MySQL**: Relational database used for storing car data and handling reservations.
- **Windows API (Sleep)**: Used to manage delays and loading times in the console application.

## Database Structure

The `cars` table includes:
- `Serial` (INT): Unique identifier for each car.
- `Brand` (VARCHAR): Car manufacturer.
- `Model` (VARCHAR): Car model.
- `Rent` (INT): Rental price per day.
- `Avail` (BOOLEAN): Availability status (true = available, false = booked).

### Sample MySQL Table

```sql
CREATE TABLE cars (
    Serial INT PRIMARY KEY,
    Brand VARCHAR(255),
    Model VARCHAR(255),
    Rent INT,
    Avail BOOLEAN
);
