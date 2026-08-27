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

**Data Selection and Filtering**

-   **Selecting a Column:** `df['column_name']` (returns a Series)
-   **Selecting Multiple Columns:** `df[['col1', 'col2']]` (returns a DataFrame)
-   **Filtering Rows (Boolean Indexing):** `df[df['Age'] > 25]` to return only rows matching the condition.
-   **Label-based Indexing:** `df.loc[:, 'col1':'col3']` to select by column or row names.
-   **Position-based Indexing:** `df.iloc[0:5, 0:3]` to select by integer index positions.

**Essential Data Cleaning**

-   **Dropping Unnecessary Columns:** `df.drop(columns=['unwanted_column'], inplace=True)`
-   **Renaming Columns:** `df.rename(columns={'old_name': 'new_name'}, inplace=True)`
-   **Checking for Duplicates:** `df.duplicated().sum()` to see how many duplicate rows exist.
-   **Dropping Duplicates:** `df.drop_duplicates(inplace=True)`

**Quick Statistics and Analysis**

-   **Summary Statistics:** `df.describe()` (generates count, mean, standard deviation, min, max, and quartiles for numerical data).
-   **Counting Unique Categories:** `df['category_column'].value_counts()`
-   **Finding Unique Elements:** `df['category_column'].unique()`

**Built-in Data Visualization**

-   **Line Plots:** `df.plot(kind='line')`
-   **Bar Charts:** `df['category'].value_counts().plot(kind='bar')`
-   **Histograms:** `df['Age'].plot(kind='hist')` to see the distribution of numerical data.