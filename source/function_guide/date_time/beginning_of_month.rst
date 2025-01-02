Beginning of Month
===

**Description:**

Returns the 1st day of the month from a specified date column.

**Function:**

.. code-block:: python

    BegMonth(table = string, col = string, new_col = string)

**Parameters:**

- *Table:* Table name on which to perform function
- *Date Column:* Column to select to find the 1st day of the month
- *New Column Name:* Name for the new column

**Example:**

.. code-block:: python

   BegMonth(table = Budget, col = "Date", new_col = "Beg of Month")

.. table:: Before

   +------------+--------+
   | Date       | Revenue|
   +============+========+
   | 1/5/2024   | 950    |
   +------------+--------+
   | 2/15/2024  | 800    |
   +------------+--------+
   | 3/31/2024  | 1200   |
   +------------+--------+

.. table:: Before

   +------------+--------+--------------+
   | Date       | Revenue| Beg of Month |
   +============+========+==============+
   | 1/5/2024   | 950    | 1/1/2024     |
   +------------+--------+--------------+
   | 2/15/2024  | 800    | 2/1/2024     |
   +------------+--------+--------------+
   | 3/31/2024  | 1200   | 3/1/2024     |
   +------------+--------+--------------+