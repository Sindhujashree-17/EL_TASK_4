# EL_TASK_4
E-Commerce Database Analysis – PostgreSQL
📌 Project Overview
This project is part of my internship, focusing on performing SQL-based data analysis on an E-Commerce Database using PostgreSQL.
The database contains key tables for managing customers, products, categories, orders, and order items.
The goal is to extract meaningful insights, optimize queries, and present the results in both tabular and visual formats.

🗂 Dataset Details
The database includes the following tables:

customers – Stores customer details (name, city, email, etc.)

categories – Stores product category names

products – Stores product details with category references

orders – Stores order details including customer reference and total amount

order_items – Stores individual product items per order

⚙️ Setup Instructions
1. Create Database
sql
Copy
Edit
CREATE DATABASE ecommerce;
2. Import CSV Files
Truncate before import to avoid key conflicts:

sql
Copy
Edit
TRUNCATE TABLE table_name RESTART IDENTITY CASCADE;
\copy table_name FROM 'C:/path/to/file.csv' DELIMITER ',' CSV HEADER;
Import files in this order:

customers

categories

products

orders

order_items

📜 SQL Queries Performed
The following queries were executed:

List customers from a specific city

Top 10 most expensive products

Total revenue per category

Customers with more than 5 orders

Order details (INNER JOIN)

All customers and their orders (LEFT JOIN)

Products with no sales

Top 5 customers by total spend (subquery)

Monthly revenue view (CREATE VIEW)


📈 Key Insights
Certain categories generate a majority of revenue.

A small group of customers contribute significantly to total sales.

Monthly sales trends help identify seasonal peaks.

🖥 Tools Used
PostgreSQL 17

pgAdmin 4
This project improved my understanding of SQL query writing, joins, views, indexing, and performance optimization.
It also enhanced my skills in turning raw database outputs into business insights through visual dashboards.
