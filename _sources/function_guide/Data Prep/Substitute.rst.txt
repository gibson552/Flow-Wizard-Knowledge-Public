Substitute
========

**Description:**

Replace one specified string or integer with another in one or many columns.
*Note: If performed on a integer or date column it will convert that column into a string*

**Function:**

.. code-block:: python

   Substitute(table = string, cols = list, search_for = string, replace_with = string)

**Parameters:**

- *Table:* Table name on which to perform function
- *Column(s):* Column(s) to substitute strings
- *Search For:* String/integer/date to find to replace
- *Replace With:* String to replace with


**Example:**

.. code-block:: python

   Substitute(table = Budget, cols = ["Geo"], search_for = "USA", replace_with = "United States")

.. table:: Before

   +----------+---------------------------+---------------+------+-------+
   | Date     | Geo                       | Business      | Plan | Actual|
   +==========+===========================+===============+======+=======+
   | 8/1/2024 | USA                       | Energy        | 800  | 850   |
   +----------+---------------------------+---------------+------+-------+
   | 7/1/2024 | USA                       | Healthcare    | 1200 | 900   |
   +----------+---------------------------+---------------+------+-------+
   | 5/1/2024 | Latin America             | Manufacturing | 900  | 1050  |
   +----------+---------------------------+---------------+------+-------+
   | 9/1/2024 | Asia-Pacific              | Technology    | 1500 | 750   |
   +----------+---------------------------+---------------+------+-------+
   | 11/1/2024| Latin America             | Energy        | 2000 | 1800  |
   +----------+---------------------------+---------------+------+-------+

.. table:: After

   +----------+---------------------------+---------------+------+-------+
   | Date     | Geo                       | Business      | Plan | Actual|
   +==========+===========================+===============+======+=======+
   | 8/1/2024 | United States             | Energy        | 800  | 750   |
   +----------+---------------------------+---------------+------+-------+
   | 9/1/2024 | United States             | Healthcare    | 1500 | 850   |
   +----------+---------------------------+---------------+------+-------+
   | 7/1/2024 | Latin America             | Manufacturing | 1200 | 900   |
   +----------+---------------------------+---------------+------+-------+
   | 5/1/2024 | Asia-Pacific              | Technology    | 900  | 1050  |
   +----------+---------------------------+---------------+------+-------+
   | 11/1/2024| Latin America             | Energy        | 2000 | 1800  |
   +----------+---------------------------+---------------+------+-------+