# Discount Impact Analytics (Jupyter + MySQL)

This project analyzes how discounts affect revenue by comparing gross revenue (before discounts), total discounts given to customers, and net revenue (after discounts). The goal is to understand whether discounts improve sales performance or simply reduce revenue.

## Overview
Discounts are a common sales strategy, but they come at a cost. This analysis evaluates discount effectiveness at a daily level using order and order-item data stored in MySQL and analyzed in a Jupyter Notebook.

## Files
- `discount_impact_analysis.ipynb` — Main analysis notebook  
- `orders.csv` — Order-level data  
- `order_items.csv` — Line-item data with pricing and discounts  
- `daily_discount_metrics.csv` — Final daily aggregated metrics  

## Key Metrics
- **Gross Revenue** = Σ(qty × unit_price)  
- **Total Discount** = Σ(qty × discount)  
- **Net Revenue** = Gross Revenue − Total Discount  
- **Discount Rate (%)** = (Total Discount ÷ Gross Revenue) × 100  

## How to Run
1. Start MySQL and create the database:
   ```sql
   CREATE DATABASE discount_impact;
