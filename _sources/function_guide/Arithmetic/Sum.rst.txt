Sum
===

**Description:**

Sums together specified columns.

**Function:**

.. code-block:: python

    Sum(Table = string, columns_to_sum = list, new_col = string)

**Parameters:**

- *Table:* Table name on which to perform function
- *Columns to Sum:* Column names to sum
- *New Column Name:* Name for the new column

**Example:**

.. code-block:: python

   Sum(table = Budget, columns_to_sum = ["Actual","Plan"], new_col = "Sum")

.. table:: Before

   +-------------------+----------------------+---------------+------+---------+
   | Date              | Geo                  | Business      | Plan | Actual  |
   +===================+======================+===============+======+=========+
   | 5/1/2024          | Latin America        | Energy        | 900  | 900     |
   +-------------------+----------------------+---------------+------+---------+
   | 5/1/2024          | Latin America        | Manufacturing | 1050 | 1100    |
   +-------------------+----------------------+---------------+------+---------+
   | 6/1/2024          | Latin America        | Energy        | 1850 | 2000    |
   +-------------------+----------------------+---------------+------+---------+


.. table:: After

   +-------------------+----------------------+---------------+------+---------+-----------+
   | Date              | Geo                  | Business      | Plan | Actual  | Sum       |
   +===================+======================+===============+======+=========+===========+
   | 5/1/2024          | Latin America        | Energy        | 900  | 900     | 1800      |
   +-------------------+----------------------+---------------+------+---------+-----------+
   | 5/1/2024          | Latin America        | Manufacturing | 1050 | 1100    | 2150      |
   +-------------------+----------------------+---------------+------+---------+-----------+
   | 6/1/2024          | Latin America        | Energy        | 1850 | 2000    | 3850      |
   +-------------------+----------------------+---------------+------+---------+-----------+
