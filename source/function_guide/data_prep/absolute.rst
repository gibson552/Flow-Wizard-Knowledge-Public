Absolute
========

**Description:**

Returns the absolute value of a number

**Function:**

.. code-block:: python

    Absolute(table = string, col = string, new_col = string)

**Parameters:**

- *Table:* Table name on which to perform function
- *Column:* Column to perform Absolute
- *New Column:* New Column Name

**Example:**

.. code-block:: python

   GroupBy(table = Budget, cols = ["Geo", "Business Unit"], agg_group = {value = "Actual", method = "sum"}, new_table_name = "Sum")

.. table:: Before

   +-------------------+----------------------+---------------+------+---------+
   | Date              | Geo                  | Business      | Plan | Actual  |
   +===================+======================+===============+======+=========+
   | 5/1/2024          | Latin America        | Energy        | 900  | -900    |
   +-------------------+----------------------+---------------+------+---------+
   | 5/1/2024          | Latin America        | Manufacturing | 1050 | 1100    |
   +-------------------+----------------------+---------------+------+---------+
   | 6/1/2024          | Latin America        | Manufacturing | 2000 | -1800   |
   +-------------------+----------------------+---------------+------+---------+

.. table:: After

   +-------------------+----------------------+---------------+------+---------+------+
   | Date              | Geo                  | Business      | Plan | Actual  | Abs  |
   +===================+======================+===============+======+=========+======+
   | 5/1/2024          | Latin America        | Energy        | 900  | -900    | 900  |
   +-------------------+----------------------+---------------+------+---------+------+
   | 5/1/2024          | Latin America        | Manufacturing | 1050 | 1100    | 1100 |
   +-------------------+----------------------+---------------+------+---------+------+
   | 6/1/2024          | Latin America        | Manufacturing | 2000 | -1800   | 1800 |
   +-------------------+----------------------+---------------+------+---------+------+