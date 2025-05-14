# Mint Classics Inventory Analysis

This repository contains an inventory and sales analysis for **Mint Classics Company**, focused on optimizing warehouse operations through SQL-based data analysis.

## Objective
To provide actionable insights for closing one of the warehouses by:
- Identifying non-selling and low-performing products
- Analyzing warehouse inventory levels
- Recommending stock redistribution strategies
- Simulating inventory reductions

## Data Overview
**Database Tables Used:**
- `products`
- `warehouses`
- `orderdetails`

**Key Fields:**
- `productCode`, `quantityInStock`, `buyPrice`
- `warehouseCode`, `warehouseName`
- `quantityOrdered`

## Business & Analysis Goals
- Optimize inventory for better cost-efficiency
- Maintain 24-hour order fulfillment post-warehouse closure
- Reduce overstocking and storage of non-moving products

## SQL Analysis Summary

1. **Product-Warehouse Mapping**  
   Understanding which products are stored in which warehouse.

2. **Warehouse Stock Summary**  
   Count of products and total stock per warehouse to determine load and performance.

3. **Non-Selling Products**  
   Identified products that have never been ordered (candidates for removal).

4. **Sales Performance**
   - Low-performing: Products with fewer than 10 units sold.
   - Top-performing: Top 10 best-sellers to be prioritized in inventory.

5. **Inventory vs. Sales**  
   Comparison to detect overstocking and adjust accordingly.

6. **5% Inventory Reduction Simulation**  
   What-if analysis to evaluate feasibility of warehouse downsizing.

7. **Unsold Product Concentration by Warehouse**  
   Identifying warehouses storing the most unsold stock.

## Recommendations

- Close underperforming warehouse(s) with the highest share of unsold products.
- Discontinue or discount non-selling/low-selling items.
- Reallocate top-selling stock across active warehouses.
- Balance inventory with actual sales trends.
- Review pricing of expensive, slow-moving products.

## Tools Used
- **SQL** for data extraction and analysis
- **Spreadsheets/Charts** for visualization (included in the report)
