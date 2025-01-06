Pivot Table
===========

**Description:**

Pivots the specified data into a table.

**Function:**

.. code-block:: python

    Pivot_table(table = string, cols = list, rows = string, agg_group = drop down, new_table_name = string)

**Parameters:**

- *Table:* Table name on which to perform function
- *Columns:* Columns of the Pivot Table
- *Rows:* Rows of the Pivot table
- *Value:* How to aggregate the numeric data (sum, count, average, median, max, min)
- *New Table Name:* Name of the Pivot Table

**Example:**

.. code-block:: python

   Pivot_Table(table = Budget, cols = ["Geo"], rows = ["Business Unit"], agg_group = {value = "Actual", method = "sum"}, new_table_name = "Pivot")

.. table:: Before

   +-------------------+----------------------+---------------+------+---------+
   | Date              | Geo                  | Business      | Plan | Actual  |
   +===================+======================+===============+======+=========+
   | 8/1/2024          | Asia-Pacific         | Energy        | 800  | 750     |
   +-------------------+----------------------+---------------+------+---------+
   | 7/1/2024          | Middle East & Africa | Healthcare    | 1200 | 900     |
   +-------------------+----------------------+---------------+------+---------+
   | 5/1/2024          | Latin America        | Manufacturing | 900  | 800     |
   +-------------------+----------------------+---------------+------+---------+
   | 9/1/2024          | Asia-Pacific         | Technology    | 1500 | 1300    |
   +-------------------+----------------------+---------------+------+---------+
   | 11/1/2024         | Latin America        | Energy        | 2000 | 1800    |
   +-------------------+----------------------+---------------+------+---------+

.. table:: After

   +---------------+-------------------+----------------------+----------------------+
   | Business Unit | Actual_Asia-Pacific | Actual_Latin America | Actual_Middle East |
   +===============+====================+=====================+======================+
   | Energy        | 750                | 1800                |                      |
   +---------------+--------------------+---------------------+----------------------+
   | Healthcare    |                    |                     | 900                  |
   +---------------+--------------------+---------------------+----------------------+
   | Manufacturing |                    | 900                 |                      |
   +---------------+--------------------+---------------------+----------------------+
   | Technology    | 1300               |                     |                      |
   +---------------+--------------------+---------------------+----------------------+