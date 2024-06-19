---
sidebar_position: 3
---

# Don'ts

1.  **Avoid SELECT `*`:** <br/>
    Don't use `SELECT *` in production queries. Explicitly list the columns you need to avoid unnecessary data transfer.

    ```sql
    SELECT * FROM users; ❌

    SELECT id, name FROM users; ✅
    ```

2.  **Avoid Long-Running Transactions:** <br/>
    Don't keep transactions open for a long time. Commit or rollback transactions as soon as possible to avoid blocking other transactions.

3.  **Avoid Excessive Indexing:** <br/>
    Don't create too many indexes on a table. Only create indexes on columns that are frequently used in WHERE clauses or JOIN conditions.

4.  **Avoid Storing Sensitive Information in Plain Text:** <br/>
    Don't store sensitive information like passwords in plain text. Use hashing algorithms like SHA-256 for storing passwords securely.
    ```sql
    CREATE TABLE users (
    username VARCHAR(50),
    password_hash CHAR(64) ❌
    );
    ```

    ```
5.  **Avoid Unnecessary Data Denormalization:** <br/>
    Don't denormalize your database schema unnecessarily. Normalize your data to reduce redundancy and improve data integrity.

        ```sql
        CREATE TABLE users (
           id SERIAL PRIMARY KEY,
           username VARCHAR(50),
           email VARCHAR(100) UNIQUE

        );
        CREATE TABLE orders (
        id SERIAL PRIMARY KEY,
        user_id INT REFERENCES users(id),
        total_amount DECIMAL(10, 2)
        );
    ```
