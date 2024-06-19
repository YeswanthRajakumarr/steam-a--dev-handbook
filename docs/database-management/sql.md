---
sidebar_position: 1
---

# SQL (postgres)

SQL (Structured Query Language) is a domain-specific programming language designed for managing and manipulating relational databases. It provides a standardized syntax and set of commands for performing various operations on databases, including querying, updating, inserting, deleting, and managing database schemas. SQL enables users to interact with databases to retrieve, modify, and manage data efficiently.

## Quick Examples

1. **Insert Data into Table:** <br/>
   ```sql
   INSERT INTO users (name, email) VALUES ('John Doe', 'john@example.com');
   ```
2. **Update Data in Table:** <br/>
   ```sql
   UPDATE users SET name = 'Jane Smith' WHERE id = 1;
   ```
3. **Delete Data from Table:** <br/>
   ```sql
   DELETE FROM users WHERE id = 1;
   ```
4. **Select Data from Table:** <br/>
   ```sql
   SELECT * FROM users WHERE id = 1;
   ```
5. **Aggregate Functions:** <br/>
   ```sql
   SELECT COUNT(*) FROM users;
   ```
6. **Joins:** <br/>

   ```sql
   SELECT u.name, o.total_amount FROM users u
    INNER JOIN orders o ON u.id = o.user_id
   ```

7. **Subqueries:** <br/>

   ```sql
   SELECT * FROM users WHERE id IN (SELECT user_id FROM orders WHERE total_amount >
   100);
   ```

8. **Group By:** <br/>

   ```sql
   SELECT city, COUNT(*) FROM customers GROUP BY city;
   ```

9. **Limit and Offset:** <br/>
   ```sql
   SELECT * FROM users LIMIT 10 OFFSET 20;
   ```
10. **Order By:** <br/>
    ```sql
    SELECT * FROM users ORDER BY created_at DESC;
    ```
11. **Distinct:** <br/>

    ```sql
    SELECT DISTINCT department FROM employees;
    ```

12. **Conditional Aggregation:** <br/>
    ```sql
    SELECT department, AVG(salary) FROM employees GROUP BY department
    ```
