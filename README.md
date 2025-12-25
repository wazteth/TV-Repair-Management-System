# TV-Repair-Management-System
This Java-based desktop application is designed for a Singapore-based TV Repair Private Company to manage its records across international stores. The system provides a graphical interface for administrative tasks, including database table management, product inventory tracking, and customer data handling.

## Features

1. **Secure Authentication**

- **Login System**: Requires administrative or user credentials to access the main menu.
- **Error Handling**: Includes specific error messaging for incorrect credentials via try-catch blocks.

2. **Database Management (Dynamic Schema)**

- **Table Creation**: Users can dynamically create new database tables by defining columns and data types directly from the UI.

- **Schema Modification**: Supports adding new columns, modifying existing ones, or deleting entire tables.

3. **Core Modules**

- **Manage Product**: Full CRUD (Create, Read, Update, Delete) operations for the `products` database table. Includes a search function by Product ID.

- **Manage Customer**: Dedicated form for handling customer records (Names, Addresses, Contact info, etc.) from the `customer` table.

- **Data Modification**: A flexible form that allows users to select any table they have created and modify its internal data.

## Technologies Used

- **Language**: Java 

- **GUI Framework**: Java Swing 

- **IDE**: NetBeans (Project Structure)

- **Database**: MySQL 


## Database Setup
The project uses a database named `repairdb`. To set up the environment:

1. Open your MySQL management tool (e.g., MySQL Workbench or Command Line).

2. Import the provided `repairdb.sql` file to create the necessary tables and initial data.

3. The default schema includes:

- `customer`: Stores details like `Customer_Name`, `Customer_Add`, and `Customer_Tel`.

- `products`: Stores inventory information.

- `user_login`: Contains authentication credentials.

## Getting Started

### Prerequisites
- Java Development Kit (JDK) 8 or higher.

- MySQL Server 8.0.

- NetBeans IDE.

### Installation
1. Clone this repository to your local machine.

2. Open NetBeans IDE and select **File > Open Project**.

3. Navigate to the cloned folder and open the project.

4. Add the **MySQL JDBC Driver** to the project libraries to ensure database connectivity.

5. Update the database connection string in the source code (typically in the login or database connection class) with your MySQL username and password.

## Project Structure

- `src/`: Contains the Java source files for Swing forms and logic.


- `repairdb.sql`: The database dump file for environment setup.


- `Documentation/`: Detailed assignment report and system overview.
