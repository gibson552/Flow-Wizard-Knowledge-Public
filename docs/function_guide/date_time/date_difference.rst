Date Difference
===

**Description:**

Calculates the difference between two date columns and returns the result as a new column.

**Function:**

.. code-block:: python

    DateDiff(table = string, start_col = string, compare_col = string, new_col = string)

**Parameters:**

- *Table:* Table name on which to perform the function
- *Start Column:* The column representing the starting date
- *Column to Compare:* The column representing the date to compare against the start column
- *New Column Name:* Name for the new column that will store the date difference

**Example:**

.. code-block:: python

   DateDiff(table = Sales_Commish_Detail, start_col = "Beg of Month", compare_col = "End of Month", new_col = "Dt Diff")

.. table:: Before

   +--------------+---------------+--------+
   | Beg of Month | End of Month  | Revenue|
   +==============+===============+========+
   | 1/1/2024     | 1/31/2024     | 950    |
   +--------------+---------------+--------+
   | 2/1/2024     | 2/28/2024     | 800    |
   +--------------+---------------+--------+
   | 3/1/2024     | 3/31/2024     | 1200   |
   +--------------+---------------+--------+

.. table:: After

   +--------------+---------------+--------+---------+
   | Beg of Month | End of Month  | Revenue| Dt Diff |
   +==============+===============+========+=========+
   | 1/1/2024     | 1/31/2024     | 950    | 30      |
   +--------------+---------------+--------+---------+
   | 2/1/2024     | 2/28/2024     | 800    | 27      |
   +--------------+---------------+--------+---------+
   | 3/1/2024     | 3/31/2024     | 1200   | 30      |
   +--------------+---------------+--------+---------+
