# Pandas Practice Notebook

Pandas is an open-source Python library designed for **data manipulation and analysis**. It makes working with structured data **fast, flexible, and intuitive** — especially if you're dealing with CSV files, Excel sheets, SQL tables, JSON, or APIs.

The two core data structures in Pandas are:

- `Series`: A 1D labeled array (like a column)
- `DataFrame`: A 2D labeled data structure (like a full spreadsheet or SQL table)

Key Features of Pandas

-   **Handling Missing Data:** Easily find, remove, or replace missing values (`NaN`).
-   **Grouping and Aggregating:** Split data into groups to calculate sums, averages, or counts quickly using `groupby`.
-   **Merging and Joining:** Combine different datasets together using SQL-style joins.
-   **Fast Input and Output:** Read and write data directly to CSV, Excel, SQL databases, and JSON files. 

Common First Steps in a Notebook

-   **Import the library:** `import pandas as pd`
-   **Load your file:** `df = pd.read_csv('filename.csv')`
-   **Check the first few rows:** `df.head()`
-   **View summary information:** `df.info()`
