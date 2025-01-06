Top K Values
============

**Description:**

Return the nth number of top values for a column

**Function:**

.. code-block:: python

    Top_Values(table = string, col = string, num_values = integer, new_table_name = string)

**Parameters:**

- *Table:* Table name on which to perform function
- *col:* Column for which to return the top
- *num_values:* The number of rows to return for with top values. For example, if you want the top 5 values, input the number 5
- *new_table_name:* The name of the new table with the nth number of top values

**Example:**

.. code-block:: python

   Top_Values(table = Budget, col = "Actual", num_values = 3, new_table_name = "Top Actual")

.. table:: Before

   =================  ======================  ===============  ======  ========
   Date               Geo                     Business         Plan    Actual
   =================  ======================  ===============  ======  ========
   7/18/2024          Middle East             Healthcare       1200    900
   5/8/2024           Latin America           Manufacturing    900     1050
   8/25/2024          Asia-Pacific            Energy           800     750
   6/15/2024          Europe                  Banking          1500    1300
   9/1/2024           North America           Retail           2000    1800
   =================  ======================  ===============  ======  ========


.. table:: After

   +-------------------+----------------------+-------------------+------+---------+
   | Date              | Geo                  | Business          | Plan | Actual  |
   +===================+======================+===================+======+=========+
   | 5/8/2024          | Latin America        | Manufacturing     | 900  | 1050    |
   +-------------------+----------------------+-------------------+------+---------+
   | 7/18/2024         | Middle East          | Healthcare        | 1200 | 900     |
   +-------------------+----------------------+-------------------+------+---------+
   | 8/25/2024         | Asia-Pacific         | Energy            | 800  | 750     |
   +-------------------+----------------------+-------------------+------+---------+
