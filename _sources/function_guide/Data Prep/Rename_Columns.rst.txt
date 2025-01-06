Rename Column(s)
========

**Description:**

Rename column name(s)

**Function:**

.. code-block:: python

   Rename_Columns(table = string, rename_group = {col = string, new_name = string} and ...)

**Parameters:**

- *Table:* Table name on which to perform function
- *Column:* Column to rename
- *New Name:* Name for new column

**Example:**

.. code-block:: python

   Rename_Columns(table = Budget, rename_group = {col = "Revenue", new_name = "MRR"} and {col = "Date", new_name = "Month" })

.. table:: Before

   +----------+---------------------------+--------+
   | Date     | Geo                       | Revenue|
   +==========+===========================+========+
   | 1/1/2024 | Geo_USA_country           | 950    |
   +----------+---------------------------+--------+
   | 2/1/2024 | Geo_USA_country           | 800    |
   +----------+---------------------------+--------+
   | 3/1/2024 | Geo_USA_country           | 1200   |
   +----------+---------------------------+--------+
   | 4/1/2024 | Geo_USA_country           | 900    |
   +----------+---------------------------+--------+


.. table:: After

   +----------+------+---------------+-------+
   | Month    | Geo  | Business      | MRR   |
   +==========+======+===============+=======+
   | 1/1/2024 | USA  | Energy        | 950   |
   +----------+------+---------------+-------+
   | 2/1/2024 | USA  | Manufacturing | 800   |
   +----------+------+---------------+-------+
   | 3/1/2024 | USA  | Energy        | 1200  |
   +----------+------+---------------+-------+
   | 4/1/2024 | USA  | Manufacturing | 900   |
   +----------+------+---------------+-------+
