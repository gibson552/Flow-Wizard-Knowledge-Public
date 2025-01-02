Group Data
==========

**Description:**

Evaluate a set of conditions and return a specific result based on the first condition that is true. This is similar to a "CASE" statement in SQL.

**Function:**

.. code-block:: python

    Groups(table = string, col = string, data_group = {logical_choice = drop down, value = string, then = string}, else_value = string, new_col = string)

**Parameters:**

- *Table:* Table name on which to perform the function
- *Column to Group:* Column to evaluate
- *Data Group:* Multiple groups of conditions can be defined.
    - *Logical Selection:* Method to evaluate (e.g., "equals", "greater than", "Is before date", etc.)
    - *Value:* The value to evaluate in the column selected to group (e.g., find "USA" in column "Geo")
    - *Then:* The value to replace the evaluated value with (e.g., replace "USA" with "United States")
- *Else Value:* The default value to use if no conditions are met
- *New Column Name:* The name for the new column that will store the result of the grouping

**Example:**

.. code-block:: python

    Groups(table = Budget, col = "Geo",
           data_group = {
               logical_choice = "Equals", value = "USA", then = "United States",
               logical_choice = "Equals", value = "CA", then = "Canada"
           },
           else_value = "Latin America", new_col = "Geo Cleaned")

.. table:: Before

   +------------+---------+------+---------+
   | Date       | Geo     | Plan | Actual  |
   +============+=========+======+=========+
   | 8/22/2023  | Canada  | 1200 | 900     |
   +------------+---------+------+---------+
   | 9/1/2022   | Columbia| 1150 | 1000    |
   +------------+---------+------+---------+
   | 8/31/2022  | Columbia| 2000 | 1800    |
   +------------+---------+------+---------+
   | 2/13/2023  | USA     | 1850 | 2000    |
   +------------+---------+------+---------+
   | 2/15/2024  | Canada  | 900  | 900     |
   +------------+---------+------+---------+
   | 7/16/2024  | Canada  | 1050 | 1100    |
   +------------+---------+------+---------+
   | 10/8/2024  | USA     | 1500 | 1300    |
   +------------+---------+------+---------+
   | 6/10/2024  | USA     | 1700 | 1400    |
   +------------+---------+------+---------+
   | 9/3/2024   | Brazil  | 800  | 750     |
   +------------+---------+------+---------+
   | 8/2/2024   | USA     | 950  | 1050    |
   +------------+---------+------+---------+

.. table:: Before

   +------------+----------+------+---------+---------------+
   | Date       | Geo      | Plan | Actual  | Geo Clean     |
   +============+==========+======+=========+===============+
   | 8/22/2023  | Canada   | 1200 | 900     | Canada        |
   +------------+----------+------+---------+---------------+
   | 9/1/2022   | USA      | 1150 | 1000    | United States |
   +------------+----------+------+---------+---------------+
   | 8/31/2022  | Columbia | 2000 | 1800    | Latin America |
   +------------+----------+------+---------+---------------+
   | 2/22/2023  | USA      | 1850 | 2000    | United States |
   +------------+----------+------+---------+---------------+
   | 2/5/2024   | Canada   | 900  | 900     | Canada        |
   +------------+----------+------+---------+---------------+
   | 7/26/2024  | Canada   | 1050 | 1100    | Canada        |
   +------------+----------+------+---------+---------------+
   | 10/8/2024  | USA      | 1500 | 1300    | United States |
   +------------+----------+------+---------+---------------+
   | 6/20/2024  | USA      | 1700 | 1400    | United States |
   +------------+----------+------+---------+---------------+
   | 9/23/2024  | Brazil   | 800  | 750     | Latin America |
   +------------+----------+------+---------+---------------+
   | 8/2/2024   | USA      | 950  | 1050    | United States |
   +------------+----------+------+---------+---------------+