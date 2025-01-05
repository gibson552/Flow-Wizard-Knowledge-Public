Round
========

**Description:**

Round decimals from an integer to the nth position

**Function:**

.. code-block:: python

   Round(table = string, cols = list, rounding = integer)

**Parameters:**

- *Table:* Table name on which to perform function
- *Columns to Round:* Columns to round
- *Number of Decimals:* nth position to round the column(s)


**Example:**

.. code-block:: python

   Round(table = Budget, cols = ["Revenue"], rounding = 2)

.. table:: Before

   +----------+---------------+------+----------+
   | Date     | Business      | Geo  | Revenue  |
   +==========+===============+======+==========+
   | 1/1/2024 | Energy        | USA  | 950.563  |
   +----------+---------------+------+----------+
   | 2/1/2024 | Manufacturing | USA  | 800.399  |
   +----------+---------------+------+----------+
   | 3/1/2024 | Energy        | USA  | 1200.123 |
   +----------+---------------+------+----------+
   | 4/1/2024 | Manufacturing | USA  | 900.985  |
   +----------+---------------+------+----------+

.. table:: After

   +----------+---------------+------+----------+
   | Date     | Business      | Geo  | Revenue  |
   +==========+===============+======+==========+
   | 1/1/2024 | Energy        | USA  | 950.56   |
   +----------+---------------+------+----------+
   | 2/1/2024 | Manufacturing | USA  | 800.601  |
   +----------+---------------+------+----------+
   | 3/1/2024 | Energy        | USA  | 1200.12  |
   +----------+---------------+------+----------+
   | 4/1/2024 | Manufacturing | USA  | 900.99   |
   +----------+---------------+------+----------+