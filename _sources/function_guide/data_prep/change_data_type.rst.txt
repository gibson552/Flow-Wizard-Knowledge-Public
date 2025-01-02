Change Data Type
========

**Description:**

Change the data type of one or many columns.

**Function:**

.. code-block:: python

    Data_Types(table = string, dtype_group = {col = string, dtype = string} and {col = string, dtype = string} ...)

**Parameters:**

- *Table:* Table name on which to perform function
- *Column:* Value to fill the column with
- *Data Type:* Data type to change the column (string, integer, date)

**Example:**

.. code-block:: python

   Data_Types(table = Budget, dtype_group = {col = "Date", dtype = "String"} and {col = "Plan", dtype = "Integer" })

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

   +-------------------+----------------------+---------------+------+---------+
   | Date              | Geo                  | Business      | Plan | Actual  |
   +===================+======================+===============+======+=========+
   | 5/1/2024          | Latin America        | Energy        | 900  |  900    |
   +-------------------+----------------------+---------------+------+---------+
   | 5/1/2024          | Latin America        | Manufacturing | 1050 | 1100    |
   +-------------------+----------------------+---------------+------+---------+
   | 6/1/2024          | Latin America        | Manufacturing | 2000 |  1800   |
   +-------------------+----------------------+---------------+------+---------+