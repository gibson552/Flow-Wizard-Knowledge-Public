Shift Values
========

**Description:**

Shifts selected Value columns by number of rows

**Function:**

.. code-block:: python

   Shift_Values(table = string, cols = list, n_rows = integer)

**Parameters:**

- *Table:* Table name on which to perform function
- *Columns to Shift:* Columns to have the rows shifted
- *Number of Rows to Shift:* Number of rows to shift down


**Example:**

.. code-block:: python

   Shift_Values(table = Budget, cols = ["Geo"], n_rows = 1)

.. table:: Before

   +----------+---------------------------+---------------+------+-------+
   | Date     | Geo                       | Business      | Plan | Actual|
   +==========+===========================+===============+======+=======+
   | 8/1/2024 | Asia-Pacific              | Energy        | 800  | 750   |
   +----------+---------------------------+---------------+------+-------+
   | 7/1/2024 | Middle East               | Healthcare    | 1200 | 900   |
   +----------+---------------------------+---------------+------+-------+
   | 5/1/2024 | Latin America             | Manufacturing | 900  | 1050  |
   +----------+---------------------------+---------------+------+-------+
   | 9/1/2024 | Asia-Pacific              | Technology    | 1500 | 1300  |
   +----------+---------------------------+---------------+------+-------+
   | 11/1/2024| Latin America             | Energy        | 2000 | 1800  |
   +----------+---------------------------+---------------+------+-------+

.. table:: After

   +----------+---------------------------+---------------+------+-------+----------------+
   | Date     | Geo                       | Business      | Plan | Actual| Geo_shift      |
   +==========+===========================+===============+======+=======+================+
   | 8/1/2024 | Asia-Pacific              | Energy        | 800  | 750   |                |
   +----------+---------------------------+---------------+------+-------+----------------+
   | 7/1/2024 | Middle East               | Healthcare    | 1200 | 900   | Asia-Pacific   |
   +----------+---------------------------+---------------+------+-------+----------------+
   | 5/1/2024 | Latin America             | Manufacturing | 900  | 1050  | Middle East    |
   +----------+---------------------------+---------------+------+-------+----------------+
   | 9/1/2024 | Asia-Pacific              | Technology    | 1500 | 1300  | Latin America  |
   +----------+---------------------------+---------------+------+-------+----------------+
   | 11/1/2024| Latin America             | Energy        | 2000 | 1800  | Asia-Pacific   |
   +----------+---------------------------+---------------+------+-------+----------------+