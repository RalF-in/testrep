# Cafe Management System

## Overview
This is a console-based Cafe Management System implemented in C. It provides functionalities for both admin and customer interaction to manage a cafe's menu, take customer orders, and generate bills. The system uses a linked list data structure to maintain the menu items and current orders dynamically.

## Features
- Menu management by an admin (add, remove, update prices)
- Admin authentication and password management
- Display of available menu items with prices
- Customer order taking with quantity limits
- Viewing current orders and calculating total bills including a fixed donation amount
- Persistent storage of the menu in a file for data retention between sessions
- Simple and user-friendly text-based interface with colored output for better user experience

## Components and Functions
- `initialmenu`: Initializes the menu with default items on first run
- `filetomenu` / `updatefile`: Load and save menu items from/to a file
- `adminlogin` / `adminpanel`: Secure admin login and menu management panel
- `additem` / `removeitem` / `priceupdate`: Modify menu items (add/remove/update price)
- `displaymenu`: Lists all available items with prices
- `takeorder`: Allows customers to place orders by selecting item IDs and quantities
- `vieworder` / `totalbill`: Shows current order details and calculates total including donations
- `changepass`: Allows the admin to change the password securely
- `general` / `intro`: Handles customer access and the main program interface

## Installation
1. Ensure you have a C compiler installed (e.g., GCC).
2. Download the source file `CafeManagement.c`.
3. Compile the program:
   ```
   gcc -o CafeManagement CafeManagement.c
   ```
4. Run the program:
   ```
   ./CafeManagement
   ```

## Usage
- On startup, choose Admin Access to manage menu and passwords (default password management included).
- Choose Customer Panel to place orders, view menu and orders.
- Follow on-screen instructions for navigation and inputs.
- Use the Admin panel for full control over menu items.

## Notes
- The program saves menu data to `amaderproject.txt`.
- Admin password is saved in `adminpass.txt`. Default setup creates these files on first run.
- Includes a small donation feature calculated as 0.5% of the total bill.
- Input validation is implemented for numeric entries and order limits.

## Author
**Roshaed Al Fardin**
