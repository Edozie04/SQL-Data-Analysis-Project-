# ClassicModels Sales Database — SQL Project

A relational database project built from scratch using the **ClassicModels** dataset — a sample business database representing a scale model car retailer. The project covers database design, schema creation, data population, and querying across 8 interrelated tables.

---

## 🛠️ Tools & Skills
- **Language**: SQL (T-SQL / MySQL compatible)
- **Concepts**: Relational database design, primary & foreign keys, referential integrity, DDL & DML, data querying

---

## 📁 Project Structure

| File | Description |
|------|-------------|
| `Uche_Chiedozie_SQL_Project.sql` | Full project: schema creation, table alterations, data inserts, and queries |

---

## 🗂️ Database Schema

The database contains **8 tables** with enforced relationships via foreign keys:

| Table | Description |
|-------|-------------|
| `customers` | Customer details and credit limits |
| `employees` | Employee records with self-referencing manager hierarchy |
| `offices` | Global office locations |
| `orders` | Customer orders and status tracking |
| `orderdetails` | Line items per order (products, quantities, prices) |
| `payments` | Customer payment records |
| `products` | Product catalogue with buy/sell prices and stock levels |
| `productlines` | Product categories and descriptions |

### Entity Relationships
- Customers place **Orders**, which contain **Order Details** linked to **Products**
- Products belong to **Product Lines**
- Employees report to other Employees (self-join hierarchy) and are assigned to **Offices**
- Customers are managed by **Employees** (sales reps)

---

## 🔧 What the Project Covers

- **Schema Design** — Created all tables with appropriate data types, `NOT NULL` constraints, primary keys, and composite keys (`orderdetails`)
- **Referential Integrity** — Enforced foreign key relationships across all tables
- **Schema Alterations** — Used `ALTER TABLE` to modify column types post-creation
- **Data Population** — Inserted real-world representative data across all 8 tables (~7,800+ lines)
- **Data Querying** — Verified data integrity with `SELECT` statements across all tables

---

## 🚀 How to Run

1. Open your SQL environment (MySQL Workbench, SQL Server Management Studio, or similar)
2. Run the `.sql` file in order — it will:
   - Create the database
   - Create all tables
   - Insert all data
   - Run verification queries

```sql
-- Example: check all customers
SELECT * FROM customers;

-- Example: check order details
SELECT * FROM orderdetails;
```

---

## 👤 Author
**Uche Chiedozie
[GitHub](https://github.com/Edozie04)
