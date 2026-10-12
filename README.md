# SQL Data Analysis Projects

## Project Overview

This repository contains SQL analysis projects completed as part of my Data Analytics and AI course at Skillovilla. The projects use SQL to answer business questions, analyze records, rank results, and identify useful insights from datasets.

## Tools and Technologies

- SQL
- Relational databases
- Joins and filtering
- Aggregate functions
- Common Table Expressions (CTEs)
- Window functions and ranking
- Date formatting

## Projects

### 1. Airline Database Analysis

**Dataset:** AirlineDB  
**Source:** Skillovilla SQL Capstone environment

This project analyzes airline-related records, including tickets, boarding passes, bookings, flights, airports, transactions, and flight schedules.

**Business questions:**

1. How many tickets are there without boarding passes?
2. How can booking references, booking dates, and total amounts be displayed, with dates formatted as `YYYY-MM-DD`?
3. How can departure airports be ranked by the number of departing flights?

**SQL concepts used:**
- `LEFT JOIN`
- `COUNT()`
- `IS NULL`
- `TO_CHAR()`
- `GROUP BY`
- `RANK()`

**Selected results:**

| Analysis | Result |
|---|---:|
| Tickets without boarding passes | 251 |
| Booking records returned | 500 rows |
| Departure airport records ranked | 104 rows |

**Query file:** [airline_analysis.sql](airline_analysis.sql)

### 2. Bike Sharing Data Analysis

**Dataset:** Bike Sharing  
**Source:** Skillovilla SQL Capstone environment

This project analyzes store sales and product quantities to compare product performance across stores and evaluate quarterly sales.

**Business questions:**

1. Which product is the most popular in each store based on quantity sold?
2. What are the total sales for each store in each quarter, and how can stores be ranked by sales performance?

**SQL concepts used:**
- `INNER JOIN`
- `SUM()`
- `GROUP BY`
- Subqueries
- Common Table Expressions (CTEs)
- `RANK()`
- `PARTITION BY`

**Selected results:**

| Analysis | Result |
|---|---:|
| Most popular products by store | 3 rows |
| Quarterly store sales and rankings | 36 rows |

**Query file:** [bike_sharing_analysis.sql](bike_sharing_analysis.sql)

## Dataset and Source Information

The datasets were accessed through Skillovilla's SQL Capstone environment. The AirlineDB and Bike Sharing questions use different data structures and are documented separately.

Public download links and redistribution permissions for the original datasets have not been verified. The repository therefore does not claim to provide the original datasets.

## How to Run the Queries

1. Obtain authorized access to the relevant dataset and database environment.
2. Open a compatible SQL editor.
3. Load or connect to the appropriate database.
4. Open the corresponding `.sql` file.
5. Run the queries against the required tables.
6. Compare the output with the expected columns and recorded results.

The database engine and external setup requirements should be confirmed from the course environment before running the queries elsewhere.

## Skills Demonstrated

- Writing SQL queries to solve business questions
- Joining related tables
- Filtering and identifying unmatched records
- Aggregating data using `COUNT()` and `SUM()`
- Formatting dates
- Ranking records with window functions
- Using subqueries and CTEs
- Interpreting query results
- Applying analytical thinking to structured data

## Author

Diya Jain

Aspiring Data Analyst | SQL | Python | Power BI | Excel
