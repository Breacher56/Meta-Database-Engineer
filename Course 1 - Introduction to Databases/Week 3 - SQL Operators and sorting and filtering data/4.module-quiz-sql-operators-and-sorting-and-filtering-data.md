# Module quiz: SQL operators and sorting and filtering data

1. Which of the following SQL statements adds a $2.00 service fee to the total price in a table called `"Orders"`, that lists the price of orders customers placed with a store?
    -   ```sql
        SELECT total + 2 FROM the Orders TABLE;
        ```
    -   ```sql
        SELECT total + 2 FROM Orders;
        ```
    -   ```sql
        SELECT total + 2 FROM Orders TABLE;
        ```
    ```
    Answer: SELECT total + 2 FROM Orders;
    Explanation: This is the right syntax to complete this task.
    ```

2. What does the following SQL statement do?
    ```sql
    SELECT total / 2 FROM Orders;
    ```
    - It returns the value of total price column in the second row.
    - It returns the result of total price divided by 2 for each cell in the total price column
    ```
    Answer: It returns the result of total price divided by 2 for each cell in the total price column
    Explanation: It returns the result of total price divided by 2 for each cell in the total price column
    ```

3. The following SQL statement returns 2 percent of the total price:
    ```sql
    SELECT total % 2 FROM Orders;
    ```
    - True
    - False
    ```
    Answer: False
    Explanation: This SQL statement returns the remainder of the total price value divided by 2.
    ```

4. Which of the following SQL statements returns 50% of the total price? Choose all correct answers.
    -   ```sql
        SELECT total / 50% FROM Orders;
        ```
    -   ```sql
        SELECT total * 0.5 FROM Orders;
        ```
    -   ```sql
        SELECT total / 2 FROM Orders;
        ```
    -   ```sql
        SELECT total * 50 FROM Orders;
        ```
    ```
    Answer: SELECT total * 0.5 FROM Orders;
            SELECT total / 2 FROM Orders;
    Explanation: SELECT total * 0.5 FROM Orders; returns 50% from the total price by multiplying the total price by 0.5.
                 SELECT total / 2 FROM Orders; returns 50% from the total price by dividing the total price by 2.
    ```

5. Select the right SQL statement to display the values of the total prices that are greater than $140.
    -   ```sql
        SELECT total FROM Orders where total < 140;
        ```
    -   ```sql
        SELECT total FROM Orders where total >= 140;
        ```
    -   ```sql
        SELECT total FROM Orders where total > 140;
        ```
    ```
    Answer: SELECT total FROM Orders where total > 140;
    Explanation: This statement displays the values of the total prices that are greater than $140
    ```

6. Does the following SQL statements sort the result-set of the total prices in ascending or descending order?
    ```sql
    SELECT * FROM Orders ORDER BY total;
    ```
    - Ascending
    - Descending
    ```
    Answer: Ascending
    Explanation: The ORDER BY keyword in SQL sorts the records in ascending order by default.
    ```

7. The following SQL statement filters data based on ____
    ```sql
    SELECT * 
    FROM customers 
    WHERE Country = "Germany";
    ```
    - `'Germany'` column with `'country'` value
    - `'Country'` column with `'Germany'` value
    ```
    Answer: 'Country' column with 'Germany' value
    Explanation: The output result of this statement will be filtered based on the country column with Germany value.
    ```

8. In SQL you can sort records in descending order using the `DESCENDING` keyword.
    - True
    - False
    ```
    Answer: False
    Explanation: You need to use the DESC keyword.
    ```

9. The output of the following SQL query within the Orders table is: UK, UK, UK, France, France, Finland
    ```sql
    SELECT DISTINCT Country FROM Orders;
    ```
    - True
    - False
    ```
    Answer: False
    Explanation: The output result of this SQL query will be: UK, France, Finland
    ```

10. What does the following SQL statement do?
    ```sql
    SELECT * FROM Orders ORDER BY country, total;
    ```
    - Orders the result by country first then total price.
    - Orders the result by country and ignores the total price.
    ```
    Answer: Orders the result by country first then total price.
    Explanation: It orders the result by country first, but if some records have the same country, it orders them by lowest total price.
    ```