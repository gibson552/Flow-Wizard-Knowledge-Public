Reverse Columns
========

**Description:**

Flip the order of select columns or all of the columns

**Function:**

.. code-block:: python

   Reverse_Columns(table = string, cols = list)

**Parameters:**

- *Table:* Table name on which to perform function
- *Columns to Reverse:* Columns to reverse the order

**Example:**

.. code-block:: python

   Reverse_Columns(table = Budget, cols = ["Geo", "Business"])

.. table:: Before

   +----------+------+---------------+---------+
   | Date     | Geo  | Business      | Revenue |
   +==========+======+===============+=========+
   | 1/1/2024 | USA  | Energy        | 950     |
   +----------+------+---------------+---------+
   | 2/1/2024 | USA  | Manufacturing | 800     |
   +----------+------+---------------+---------+
   | 3/1/2024 | USA  | Energy        | 1200    |
   +----------+------+---------------+---------+
   | 4/1/2024 | USA  | Manufacturing | 900     |
   +----------+------+---------------+---------+

.. table:: After

   +----------+---------------+------+---------+
   | Date     | Business      | Geo  | Revenue |
   +==========+===============+======+=========+
   | 1/1/2024 | Energy        | USA  | 950     |
   +----------+---------------+------+---------+
   | 2/1/2024 | Manufacturing | USA  | 800     |
   +----------+---------------+------+---------+
   | 3/1/2024 | Energy        | USA  | 1200    |
   +----------+---------------+------+---------+
   | 4/1/2024 | Manufacturing | USA  | 900     |
   +----------+---------------+------+---------+