# MSSQL-DBA-Screening
quick one-hour assignment

## Approach

1. **Understanding Requirements**: The first step was to understand the requirements clearly. This involved identifying the necessary SQL scripts for various tasks such as retrieving last update times, inserting data, and querying specific information from the `Products` table.

2. **Writing SQL Scripts**: Based on the requirements, I wrote SQL scripts to:
   - Query the top 5 most expensive products in stock.
   - Calculate the total number of products added in the last 30 days.
   - Show the average price per category, sorted by highest to lowest.

3. **Index Optimization**: Suggested indexes to improve query performance, including a composite index to cover multiple columns.

4. **Exporting Data**: Provided a basic script using the `bcp` utility to export query results to a `.csv` file.

## Optimizations Suggested

1. **Indexing**: Recommended creating indexes on frequently queried columns (`Category`, `Price`, `InStock`) to speed up query performance. Also suggested a composite index to cover multiple columns.

2. **Query Optimization**: Ensured that queries are written efficiently, using appropriate filtering and sorting to minimize the load on the database.

3. **Execution Plan Analysis**: Provided scripts to check the execution plan using `SET SHOWPLAN_ALL` to identify potential performance bottlenecks.

## Real-World Scenario Handling

1. **Scalability**: In a real-world scenario, it's important to ensure that the database can handle large volumes of data. This involves regular monitoring and optimization of indexes and queries.

2. **Data Integrity**: Implementing constraints and triggers to maintain data integrity. For example, ensuring that `ProductID` is unique and that `Price` and `InStock` values are within reasonable ranges.

3. **Backup and Recovery**: Setting up regular backups and a recovery plan to prevent data loss.

4. **Security**: Implementing security measures such as user authentication, authorization, and encryption to protect sensitive data.

5. **Documentation**: Maintaining comprehensive documentation for all database operations, including schema design, indexing strategies, and query optimization techniques.

6. **Continuous Improvement**: Regularly reviewing and optimizing database performance based on usage patterns and feedback.
