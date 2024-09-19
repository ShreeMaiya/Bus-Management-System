# Bus Management System

## Project Overview
The **Bus Management System** is a database management system (DBMS) project designed to automate and streamline bus transportation operations. The system supports various user roles such as administrators, conductors, and drivers, each with distinct access levels and functionalities.

The project aims to replace manual and error-prone processes with an automated solution that enhances efficiency, reduces operational errors, and improves overall service delivery.

## Features
- **Admin Dashboard**: 
  - Add or manage bus, conductor, and driver information.
  - View bus schedules, revenue, and mileage details.
- **Conductor Dashboard**:
  - Manage passenger details, ticket sales, and assigned trips.
- **Driver Dashboard**:
  - Record fuel usage, travel times, and manage trip reports.
- **Passenger**:
  - View bus schedules and check timetables without login.

## Technology Stack
- **Frontend**:
  - HTML, CSS, JavaScript, Bootstrap
- **Backend**:
  - PHP
- **Database**:
  - MySQL
- **Development Environment**:
  - XAMPP

## Database Schema
The system uses MySQL as its database, with several tables to store information about buses, passengers, trips, and users (admin, conductor, driver). The main tables include:
- `Bus_Details`
- `Login_Admin`, `Login_Conductor`, `Login_Driver`
- `Passenger`
- `Trip_Incharge`
- `Trip_Real_Details`
- `Trip_Result`

Views such as `Revenueperbus` and `Mileage` provide key insights for administration.

## Installation Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/ShreeMaiya/Bus-Management-System.git
   ```

2. Set up the database:
   - Use XAMPP to start MySQL and Apache servers.
   - Create a new database called `dbms_bus_mgm`.
   - Import the SQL schema and data from the project files.

3. Configure the database connection in the `config.php` file:
   ```php
   $servername = "localhost";
   $username = "root";
   $password = "";
   $dbname = "dbms_bus_mgm";
   ```

4. Run the project:
   - Open a browser and navigate to `http://localhost/Bus-Management-System`.

## Usage
- Admin can log in using the credentials:
  - Username: `admin`
  - Password: `123`
- Conductors and drivers will have separate login credentials, as specified in the database.

## Future Enhancements
- Mobile app integration.
- GPS tracking for real-time bus location updates.
- Online ticket booking and payment gateways.
- Predictive maintenance and advanced analytics.

