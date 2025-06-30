# Apple Retail Sales SQL Project
Analyzing Millions of Rows of Sales Data


# ![Apple Logo](https://github.com/aakiffpanjwani/sql_apple/blob/main/store.jpg)

## Project Overview
I designed this project to showcase my advanced SQL querying skills by analyzing more than one million rows of Apple retail sales data. The dataset captures products, stores, sales transactions, and warranty claims from Apple retail locations around the world. By tackling questions that range from straightforward counts to complex correlation analyses, I demonstrate how I extract actionable insights from large, relational datasets.

## Entity-Relationship Diagram (ERD)
(See ERD illustration for table relationships.)

![ERD](https://github.com/aakiffpanjwani/sql_apple/blob/main/erd.png)

## Database Schema
I structured the database around five core tables:

1. **stores**: Contains information about Apple retail stores.
   - `store_id`: Unique identifier for each store.
   - `store_name`: Name of the store.
   - `city`: City where the store is located.
   - `country`: Country of the store.

2. **category**: Holds product category information.
   - `category_id`: Unique identifier for each product category.
   - `category_name`: Name of the category.

3. **products**: Details about Apple products.
   - `product_id`: Unique identifier for each product.
   - `product_name`: Name of the product.
   - `category_id`: References the category table.
   - `launch_date`: Date when the product was launched.
   - `price`: Price of the product.

4. **sales**: Stores sales transactions.
   - `sale_id`: Unique identifier for each sale.
   - `sale_date`: Date of the sale.
   - `store_id`: References the store table.
   - `product_id`: References the product table.
   - `quantity`: Number of units sold.

5. **warranty**: Contains information about warranty claims.
   - `claim_id`: Unique identifier for each warranty claim.
   - `claim_date`: Date the claim was made.
   - `sale_id`: References the sales table.
   - `repair_status`: Status of the warranty claim (e.g., Paid Repaired, Warranty Void).

## Objectives
I organized my analysis into three tiers of questions that progressively increase in complexity.

Tier 1 – Easy to Medium
1. Count the number of stores in each country.

2. Calculate total units sold per store.

3. Identify how many sales occurred in December 2023.

4. Find stores that have never had a warranty claim.

5. Determine the percentage of claims marked “Warranty Void.”

6. Reveal which store sold the most units in the last year.

7. Count unique products sold in the last year.

8. Compute the average product price per category.

9. Count warranty claims filed in 2020.

10. For each store, identify the single best-selling day (highest quantity).

Tier 2 – Medium to Hard
11. For every country and year, identify the least-selling product (by units).

12. Count claims filed within 180 days of purchase.

13. Count claims on products launched in the last two years.

14. List months (past three years) when U.S. sales exceeded 5 000 units.

15. Identify the category with the most claims in the last two years.

Tier 3 – Complex

16. Compute the probability of a warranty claim after purchase, per country.

17. Measure year-over-year growth for each store.

18. Correlate product price with warranty-claim frequency (last five years, by price band).

19. Find the store with the highest share of “Paid Repaired” claims.

20. Produce a monthly running-total sales trend for every store over the past four years.

## Project Focus
My main goal is to demonstrate:

Complex joins & aggregations – combining multiple tables to surface insights.

Window functions – running totals, growth rates, and time-series comparisons.

Time-based segmentation – slicing data into meaningful launch-age buckets.

Correlation analysis – evaluating relationships (e.g., price vs. claim likelihood).

Real-world decision support – answering questions an Apple retail analyst might face.


## Dataset Details
Size: 1,000,000 + sales rows (plus supporting tables).

Time Span: Multiple years, enabling long-term trend analysis.

Geography: Apple retail stores across numerous countries.

## Conclusion
By designing, building, and querying this dataset myself, I prove my ability to handle enterprise-scale data, craft efficient SQL, and translate raw transactions into strategic business insights.
