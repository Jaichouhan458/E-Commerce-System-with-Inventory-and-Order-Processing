# E-Commerce-System-with-Inventory-and-Order-Processing
A Python-based e-commerce system that manages users, products, orders, and payments, with integrated inventory management. Features order processing, restocking alerts, and SQL queries for insights on customer purchases and revenue. Includes database setup scripts and a connection management module

 E-Commerce System Assessment

This project implements a simplified e-commerce system that includes inventory management, order processing, and database interactions. It consists of three main parts: system design, business logic implementation, and database query handling.

## Directory Structure
- `system_design.py`: Contains the implementation of the e-commerce system with classes for Users, Products, Orders, and Payments.
- `business_logic.py`: Implements the inventory management system that tracks stock levels and processes orders.
- `database_queries.sql`: Contains SQL queries for database operations.
- `create_tables.sql`: SQL script to create the necessary tables in the MySQL database.
- `requirements.txt`: Lists the required Python libraries for the project.
- `class_diagram.png`: System design diagram.
- `query_execution.py`: Contains the connection setup and SQL queries.

## Part 1: System Design (E-Commerce System)
This part models a simplified e-commerce system where users can create and manage orders, add products, and handle payments.

### How to Run
1. Open `system_design.py`.
2. Run the script to see how a user creates an order, adds products, and makes a payment.

### Assumptions
- Users can add multiple products to an order.
- Payments are linked to specific orders.

---

## Part 2: Business Logic Implementation (Inventory Management)
This part implements an inventory management system that reduces stock levels based on incoming sales orders and triggers alerts for restocking when necessary.

### How to Run
1. Open `business_logic.py`.
2. Run the script to process sales orders and manage inventory.

### Assumptions
- If a product’s stock drops below the threshold (10 units), an alert is triggered.
- If insufficient stock is available, an error will be raised.

---

## Part 3: Database Query Handling (SQL)
open query_execution.py
This section provides SQL queries to interact with the database, including retrieving customer purchase data and calculating revenue by author.

### How to Run
- Execute the SQL queries found in `database_queries.sql` using a MySQL client to get insights from your database.

---

## Requirements
- Python 3.x
- MySQL Connector Python Library
- MySQL Database

## Setup Instructions
1. Install the required library:
   ```bash
   pip install mysql-connector-python

## Set up your MySQL database:
Create a new database using your preferred MySQL client (e.g., MySQL Workbench, command line).
Execute create_tables.sql to create the necessary tables in your database.
Update the database credentials in any relevant scripts (e.g., query_execution.py).
## Assumptions
The MySQL server is running locally.
The user has sufficient privileges to create databases and tables.
