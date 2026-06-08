# Sales Trend Analysis Using Aggregations

## 📌 Project Objective
This project focuses on analyzing monthly e-commerce revenue and order volumes from an online sales dataset. The primary goal is to practice grouping data, using aggregate functions, and analyzing time-based trends using SQL.

---

## 🛠️ Tools & Environment
* **Database Engine:** SQLite (compatible syntax provided for PostgreSQL/MySQL)
* **Platform:** [SQLiteOnline IDE](https://sqliteonline.com/)
* **Dataset:** `online_sales` (Internal Mock Data)

---

## 💾 Database Schema & Data Setup
The analysis utilizes an `orders` structure within the `online_sales` table containing the following attributes:
* `order_id`: Unique identifier for each order.
* `order_date`: The date the transaction occurred.
* `amount`: Total revenue generated from the order.
* `product_id`: Identifier for the item sold.

### Table Creation and Mock Data Script
```sql
DROP TABLE IF EXISTS online_sales;

CREATE TABLE online_sales (
    order_id INTEGER,
    order_date DATE,
    amount DECIMAL(10,2),
    product_id INTEGER
);

INSERT INTO online_sales (order_id, order_date, amount, product_id) VALUES
(1, '2026-01-15', 150.00, 10),
(2, '2026-01-22', 210.50, 11),
(3, '2026-02-05', 340.00, 10),
(4, '2026-02-18', 120.00, 12),
(5, '2026-03-02', 500.00, 11),
(6, '2026-03-25', 250.75, 10);
