Create Column
========

**Description:**

Create a new column and fill with a static value.

**Function:**

.. code-block:: python

    Create_Column(table = string, fill = string/integer/date, dtype = drop down, new_col = string)

**Parameters:**

- *Table:* Table name on which to perform function
- *Fill With:* Value to fill the column with
- *Data Type:* What the data type the column is filled with (string, integer, date)
- *New Column Name:* Name for new column

**Example:**

.. code-block:: python

   Create_Column(table = Budget, fill = "12", dtype = "Integer", new_col = "Months")

.. table:: Before

   +-------------------+----------------------+---------------+------+---------+
   | Date              | Geo                  | Business      | Plan | Actual  |
   +===================+======================+===============+======+=========+
   | 5/1/2024          | Latin America        | Energy        | 900  |  900    |
   +-------------------+----------------------+---------------+------+---------+
   | 5/1/2024          | Latin America        | Manufacturing | 1050 | 1100    |
   +-------------------+----------------------+---------------+------+---------+
   | 6/1/2024          | Latin America        | Manufacturing | 2000 |  1800   |
   +-------------------+----------------------+---------------+------+---------+

.. table:: After

   +-------------------+----------------------+---------------+------+---------+--------+
   | Date              | Geo                  | Business      | Plan | Actual  | Months |
   +===================+======================+===============+======+=========+========+
   | 5/1/2024          | Latin America        | Energy        | 900  | 900     | 12     |
   +-------------------+----------------------+---------------+------+---------+--------+
   | 5/1/2024          | Latin America        | Manufacturing | 1050 | 1100    | 12     |
   +-------------------+----------------------+---------------+------+---------+--------+
   | 6/1/2024          | Latin America        | Energy        | 1850 | 2000    | 12     |
   +-------------------+----------------------+---------------+------+---------+--------+