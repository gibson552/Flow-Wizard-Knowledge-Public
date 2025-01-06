MinIfs
======

**Description:**

Minimum values based on inputs and group. It will return a new table.

**Function:**

.. code-block:: python

    MinIfs(table = string, cols = list, min_col = string, new_table_name = string)

**Parameters:**

- *Table:* Table name on which to perform function
- *Columns:* Columns that you wish to group
- *Min Column:* Value column you wish to return the Minimum values
- *New Table Name:* Name for new table

**Example:**

.. code-block:: python

   MinIfs(table = Budget, cols = ["Geo"], max_col = "Actual", new_table_name = "MinIfs")

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

   +-------------------+---------+
   | Geo               | Actual  |
   +===================+=========+
   | Asia-Pacific      | 750     |
   +-------------------+---------+
   | Middle East & Af. | 900     |
   +-------------------+---------+
   | Latin America     | 900     |
   +-------------------+---------+