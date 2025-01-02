AverageIfs
==========

**Description:**

Average values based on inputs and group. It will return a new table.

**Function:**

.. code-block:: python

    AverageIfs(table = string, cols = list, average_col = string, new_table_name = string)

**Parameters:**

- *Table:* Table name on which to perform function
- *Columns:* Columns that you wish to group
- *Average Column:* Value column you wish to return averages
- *New Table Name:* Name for new table

**Example:**

.. code-block:: python

   AverageIfs(table = Budget, cols = [Business_Unit, Geo], average_col = Amount, new_table_name = AveragebyBU&Geo)


=====  =====  =======
A      B      A and B
=====  =====  =======
False  False  False
True   False  False
False  True   False
True   True   True
=====  =====  =======

