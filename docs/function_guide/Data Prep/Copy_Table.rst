Copy Table
========

**Description:**

Duplicate a table

**Function:**

.. code-block:: python

    Copy_Table(table = string, new_table_name = string)

**Parameters:**

- *Table:* Table name on which to perform function
- *Append Table:* Table to append to the parameter Table
- *New Table Name:* Name of the new table

**Example:**

.. code-block:: python

   Copy_Table(table = Budget, new_table_name = "Duplicate")

.. table:: Before *Budget*

   +-------------------+----------------------+---------------+------+---------+
   | Date              | Geo                  | Business      | Plan | Actual  |
   +===================+======================+===============+======+=========+
   | 5/1/2024          | Latin America        | Energy        | 900  | -900    |
   +-------------------+----------------------+---------------+------+---------+
   | 5/1/2024          | Latin America        | Manufacturing | 1050 | 1100    |
   +-------------------+----------------------+---------------+------+---------+
   | 6/1/2024          | Latin America        | Manufacturing | 2000 | -1800   |
   +-------------------+----------------------+---------------+------+---------+

.. table:: After *Duplicate*

   +-------------------+----------------------+---------------+------+---------+
   | Date              | Geo                  | Business      | Plan | Actual  |
   +===================+======================+===============+======+=========+
   | 5/1/2024          | Latin America        | Energy        | 900  | -900    |
   +-------------------+----------------------+---------------+------+---------+
   | 5/1/2024          | Latin America        | Manufacturing | 1050 | 1100    |
   +-------------------+----------------------+---------------+------+---------+
   | 6/1/2024          | Latin America        | Manufacturing | 2000 | -1800   |
   +-------------------+----------------------+---------------+------+---------+