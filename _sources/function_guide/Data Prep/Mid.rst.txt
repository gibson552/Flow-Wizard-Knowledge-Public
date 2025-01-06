Mid
========

**Description:**

Return the middle characters of a string

**Function:**

.. code-block:: python

   Mid(table = string, col = string, left_start = integer, right_start = integer, new_col = string)

**Parameters:**

- *Table:* Table name on which to perform function
- *Column Name:* Column to perform function
- *Number of Characters from left side: * How far from the left to start the Mid
- *Number of Characters from right side: * How far from the right to start the Mid
- *New Column Name:* Name for new column

**Example:**

.. code-block:: python

   Mid(table = Budget, col = "Geo", left_start = 4, right_start = 8, new_col = "Mid")

.. table:: Before

   +----------+---------------------------+-------+
   | Date     | Geo                       | Actual|
   +==========+===========================+=======+
   | 1/1/2024 | Geo_USA_country           | 950   |
   +----------+---------------------------+-------+
   | 2/1/2024 | Geo_USA_country           | 800   |
   +----------+---------------------------+-------+
   | 3/1/2024 | Geo_USA_country           | 1200  |
   +----------+---------------------------+-------+
   | 4/1/2024 | Geo_USA_country           | 900   |
   +----------+---------------------------+-------+


.. table:: After

   +----------+------+---------------+-------+
   | Date     | Geo  | Business      | Actual|
   +==========+======+===============+=======+
   | 1/1/2024 | USA  | Energy        | 950   |
   +----------+------+---------------+-------+
   | 2/1/2024 | USA  | Manufacturing | 800   |
   +----------+------+---------------+-------+
   | 3/1/2024 | USA  | Energy        | 1200  |
   +----------+------+---------------+-------+
   | 4/1/2024 | USA  | Manufacturing | 900   |
   +----------+------+---------------+-------+
