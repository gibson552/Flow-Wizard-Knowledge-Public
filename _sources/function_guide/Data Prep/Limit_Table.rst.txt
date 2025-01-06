Limit Table
========

**Description:**

Keep only the first or last n number of rows in a table. You can create a new table or overwrite the existing.

**Function:**

.. code-block:: python

    Limit_Table(table = string, n_rows = integer, source = string, new_table = checkbox, new_table_name = string)

**Parameters:**

- *Table:* Table name on which to perform function
- *Number of Rows:* Number of rows to keep
- *First/Last Number of Rows:* Keep rows from the top of the table or bottom (First/Last)
- *New Table:* Create a new table or overwrite the existing (True/False checkbox)
- *New Table Name:* Name for new table

**Example:**

.. code-block:: python

   Limit_Table(table = Budget, n_rows = 2, source = "Last", new_table = True, new_table_name = "Limited")

.. table:: Before

   +----------+--------------------------------------+------+---------+
   | Date     | Geo - BU                             | Plan | Actual  |
   +==========+======================================+======+=========+
   | Jul 2024 | Middle East & Africa - Healthcare    | 1200 | 900     |
   +----------+--------------------------------------+------+---------+
   | Jul 2024 | Middle East & Africa - Energy        | 1150 | 1000    |
   +----------+--------------------------------------+------+---------+
   | Jun 2024 | Latin America - Energy               | 2000 | 1800    |
   +----------+--------------------------------------+------+---------+
   | Jun 2024 | Latin America - Energy               | 1850 | 2000    |
   +----------+--------------------------------------+------+---------+


.. table:: After

   +----------+--------------------------------------+------+---------+-------+
   | Date     | Geo - BU                             | Plan | Actual  | Left  |
   +==========+======================================+======+=========+=======+
   | Jun 2024 | Latin America - Energy               | 2000 | 1800    | Jun   |
   +----------+--------------------------------------+------+---------+-------+
   | Jun 2024 | Latin America - Energy               | 1850 | 2000    | Jun   |
   +----------+--------------------------------------+------+---------+-------+
