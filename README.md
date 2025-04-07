# 🍽️ Online Food Ordering System

## Project Details
* **Group**: 20  
* **Roll Numbers**: 96–100

## Team Members

| Name                  | Roll Number  |
|-----------------------|--------------|
| GUGULOTHU SANDEEP     | 23CS8096     |
| LINGAMPALLY SIRIJA    | 23CS8097     |
| SATYANARAYANA         | 23CS8098     |
| YOUSUF KHAN           | 23CS8099     |
| VANSH RAJ             | 23CS8100     |

---

## 📝 Problem Statement
Develop an Online Food Ordering System that allows customers to place food orders from restaurants. The system should manage restaurant menus, customer details, order history, and allow for analytics such as top-selling items, total revenue, and customer behavior insights.

---

## 📖 About the Project

This project simulates a real-world food delivery system using **MySQL**. It includes tables for customers, restaurants, food items, orders, and ordered items. Sample data is inserted to test various SQL queries including joins, aggregations, groupings, and order analysis.

We have also included **stored procedures** for reusable queries and **triggers** for automated updates on data change.

---

## 🗃️ Database Schema

### 1. Customers
- `CustomerID` (Primary Key)
- `Name`
- `Contact`
- `Address`

### 2. Restaurants
- `RestaurantID` (Primary Key)
- `Name`
- `Location`
- `Rating`

### 3. FoodItems
- `FoodItemID` (Primary Key)
- `RestaurantID` (Foreign Key)
- `Name`
- `Price`

### 4. Orders
- `OrderID` (Primary Key)
- `CustomerID` (Foreign Key)
- `RestaurantID` (Foreign Key)
- `OrderDate`
- `TotalAmount`

### 5. OrderItems
- `OrderItemID` (Primary Key)
- `OrderID` (Foreign Key)
- `FoodItemID` (Foreign Key)
- `Quantity`

---

## 📁 File Structure

Online_Food_Ordering_System  
├── SQL_Scripts 

│   ├── createTable.sql

│   ├── insertTable.sql 

│   ├── queries.sql

│   ├── stored_procedures.sql

│   └── triggers.sql

├── Screenshots 

│   └── (All SQL query outputs) 

├── Report

│   └── DBMS_MiniProject.pdf

└── README.md


---

## ⚙️ How to Run the Project

### Using MySQL Workbench:
1. Open each `.sql` file from the **SQL_Scripts** folder in the following order:
   - `createTable.sql`
   - `insertTable.sql`
   - `queries.sql`
   - `stored_procedures.sql`
   - `triggers.sql`
2. Run each script to set up the database and test features.

### Using MySQL Command Line:
```bash
mysql -u your_username -p

### then execute:
SOURCE SQL_Scripts/createTable.sql;
SOURCE SQL_Scripts/insertTable.sql;
SOURCE SQL_Scripts/queries.sql;
SOURCE SQL_Scripts/stored_procedures.sql;
SOURCE SQL_Scripts/triggers.sql;
```

**NOTE:**
"This is our submission for the DBMS course project. We've implemented everything using MySQL as our relational database environment."
