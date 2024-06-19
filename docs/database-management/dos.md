---
sidebar_position: 2
---

# Do's

1. **Use Transactions for Data Consistency:** <br/>
   Do use transactions when performing multiple database operations to ensure data consistency and integrity.

   ```sql
   BEGIN;
   -SQL queries.....
   COMMIT;
   ```

2. **Optimize Queries for Performance:** <br/>
   Do optimize your SQL queries by using appropriate indexes, avoiding unnecessary joins, and optimizing WHERE clauses.

   ```sql
   EXPLAIN SELECT * FROM users WHERE id = 123;
   ```

3. **Use Prepared Statements to Prevent SQL Injection:** <br/>
   Do use prepared statements or parameterized queries to prevent SQL injection attacks.

   ```sql
   PREPARE get_user_by_id (INT) AS
   SELECT * FROM users WHERE id = $1;
   EXECUTE get_user_by_id(123);
   ```

4. **Regularly Back Up Your Database:** <br/>
   Do regularly back up your PostgreSQL database to prevent data loss in case of hardware failure or accidental deletion.

   ```bash
   pg_dump -U username -d dbname > backup.sql
   ```

5. **Use Views for Simplified Querying:** <br/>
   Do use views to simplify complex queries and provide a logical abstraction over your database schema.
   ```sql
   CREATE VIEW active_users AS
   SELECT * FROM users WHERE status = 'active';
   ```
6. **Implement Constraints for Data Integrity:** <br/>
   Do use constraints like NOT NULL, UNIQUE, FOREIGN KEY, etc., to maintain data integrity and enforce business rules

    ```sql
    ALTER TABLE users ADD CONSTRAINT email_unique UNIQUE (email);
    ```