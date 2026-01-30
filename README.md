# Discount Impact Analytics (Jupyter + MySQL)

This project analyzes how discounts affect revenue by comparing gross revenue (before discounts), total discounts given to customers, and net revenue (after discounts).  
The goal is to understand whether discounts improve performance or simply reduce revenue.

---

## Project Overview

Discounts are commonly used to increase sales, but they also reduce revenue.  
This analysis evaluates the impact of discounts at a daily level using order and order-item data stored in MySQL and analyzed in a Jupyter Notebook.

---

## File Structure

---

## Data Description

- **orders.csv**
  - Order-level information (order date, status)
- **order_items.csv**
  - Line-item details including quantity, unit price, and discount per unit

---

## Key Metrics

- **Gross Revenue**  
  Σ(qty × unit_price)

- **Total Discount**  
  Σ(qty × discount)

- **Net Revenue**  
  Gross Revenue − Total Discount

- **Discount Rate (%)**  
  (Total Discount ÷ Gross Revenue) × 100

---

## How to Run

1. Start MySQL and create the database:
   ```sql
   CREATE DATABASE discount_impact;
