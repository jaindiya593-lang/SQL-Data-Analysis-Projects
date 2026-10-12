# SQL-Data-Analysis-Projects

## Project Overview
This project explores airline database information using SQL. It focuses on analyzing ticket bookings and boarding-pass records to answer business questions and identify useful insights from relational data.

The project was completed as part of the Data Analytics and AI course at Skillovilla.

## Objectives
- Analyze airline ticket and boarding-pass records.
- Use SQL joins to connect related tables.
- Apply filtering and aggregate functions to answer business questions.
- Identify tickets that do not have corresponding boarding-pass records.

## Database and Tools
- **Database:** AirlineDB
- **Query language:** SQL
- **Platform:** Skillovilla SQL Capstone
- **Database engine:** To be confirmed from the course environment.

## Dataset and Source
The AirlineDB dataset is provided through the Skillovilla SQL Capstone environment. The database description identifies information related to transactions, tickets, flights, airports, and flight schedules.

The original database files and public redistribution permissions have not been verified. The project therefore references the course environment rather than offering an unverified public dataset download.

## Schema and Table Relationships
The project description identifies the following tables or data areas:

- `TICKETS` — ticket records.
- `BOARDING_PASSES` — boarding-pass records associated with tickets.
- `FLIGHTS` — flight information.
- `TRANSACTIONS` — transaction information.
- `AIRPORTS` — airport information.
- Flight schedules — scheduled flight information.

**Verified relationship used in the current query:** `TICKETS.TICKET_NO` is joined to `BOARDING_PASSES.TICKET_NO`.

The remaining table relationships should be documented after checking the actual schema. They are not assumed here.

## Business Questions
1. How many tickets are there without boarding passes?
2. What additional insights can be obtained by connecting ticket, flight, transaction, airport, and schedule data?

Further questions and their results will be added after verifying the remaining project queries.

## SQL Query and Explanation

### 1. Count tickets without boarding passes

**Business question:** How many tickets are there without boarding passes?

```sql
SELECT
    COUNT(*)
FROM TICKETS AS T
LEFT JOIN BOARDING_PASSES AS BP
    ON T.TICKET_NO = BP.TICKET_NO
WHERE BP.TICKET_NO IS NULL;
```

**Explanation:**
- `LEFT JOIN` retains ticket records even when no matching boarding-pass record exists.
- `WHERE BP.TICKET_NO IS NULL` filters for tickets without a matching boarding pass.
- `COUNT(*)` returns the number of matching ticket records.

**Result:** 251 tickets without boarding passes.

## Selected Results
| Business question | Result |
|---|---:|
| Tickets without boarding passes | 251 |

These results are based on the output displayed in the Skillovilla SQL Capstone environment.

## How to Run
1. Open the AirlineDB SQL Capstone environment in Skillovilla.
2. Access the relevant database and its tables.
3. Open the SQL editor.
4. Run the query shown above.
5. Compare the output with the recorded result.

To run the query outside Skillovilla, you will need an authorized copy of the database and a compatible SQL environment. The database engine and external setup requirements are yet to be confirmed.

## Project Files
- [SQL Analysis Queries](airline_analysis.sql) — SQL query file, to be added after preparing the permitted project queries.
- [Original Skillovilla project reference](SQL%20Project%20Link.txt) — course reference, if retained.

## Skills Demonstrated
- SQL joins (`LEFT JOIN`)
- Aggregate functions (`COUNT`)
- Filtering with `WHERE`
- Handling unmatched records using `IS NULL`
- Translating a business question into a SQL query
- Interpreting query results

## Author
Diya Jain

Entry-level Data Analyst | SQL | Python | Power BI | Excel
