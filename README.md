# Data Transformer SQL Project

## Objective

Data Transformer is a MySQL project for practicing advanced SQL
operations used in reporting and data analysis.

## Tables

-   **Customers**: customer identity, name, email, and registration
    date.
-   **Orders**: order date, amount, and the customer who placed the
    order.
-   **Employees**: employee names, department, hire date, and salary.

## Topics Covered

1.  INNER JOIN
2.  LEFT JOIN
3.  RIGHT JOIN
4.  FULL OUTER JOIN emulation using `LEFT JOIN`, `RIGHT JOIN`, and
    `UNION ALL`
5.  Subquery for orders above average amount
6.  Subquery for employees earning above average salary
7.  Extracting year and month from dates
8.  Calculating date differences with `DATEDIFF()`
9.  Formatting dates with `DATE_FORMAT()`
10. Combining names with `CONCAT()`
11. Replacing text with `REPLACE()`
12. Converting text with `UPPER()` and `LOWER()`
13. Trimming email whitespace with `TRIM()`
14. Running totals with `SUM() OVER()`
15. Ranking orders with `RANK()`
16. Discount calculation using `CASE`
17. Salary categorization using `CASE`

## Requirements

-   MySQL 8.0 or later (window functions are used).

## How to Run

1.  Open the `DATA_TRANSFORMER.sql` file in MySQL Workbench or a text
    editor.

2.  Execute the complete script using MySQL Workbench, or run it in the
    MySQL command-line client with a command such as:

    ``` sql
    SOURCE C:/full/path/to/DATA_TRANSFORMER.sql;
    ```

3.  Replace the example path with the actual path to the SQL file.

## Assumptions

-   Additional sample rows are included to demonstrate the requested
    queries.
-   Customer 4 intentionally has no orders to demonstrate `LEFT JOIN`.
-   MySQL does not support native `FULL OUTER JOIN`; it is emulated
    using a `LEFT JOIN` and unmatched rows from a `RIGHT JOIN`.
-   Salary categories: High \>= 70000, Medium \>= 50000 and \< 70000,
    Low \< 50000.
-   Discounts: amounts \> 1000 receive 10%; amounts \> 500 receive 5%;
    otherwise 0%.
-   Name replacement and email trimming are shown in `SELECT` statements
    and do not modify the stored data.

## Files

-   `DATA_TRANSFORMER.sql` --- complete executable SQL script with all
    17 tasks.
-   `DATA_TRANSFORMER_English_Reasons.txt` --- English explanations and
    reasons for each task.
