Sort Table
========

**Description:**

Sort one or many columns in a table ascending or descending in order.

**Function:**

.. code-block:: python

   Sort_Table(table = string, sort_group = {col = string, sort = string} and ...)

**Parameters:**

- *Table:* Table name on which to perform function
- *Column:* Column to sort
- *Sort:* Sort the column ascending or descending


**Example:**

.. code-block:: python

   Sort_Table(table = Budget, sort_group = {col = "Geo", sort = "Asc"} and {col = "Actual", sort = "Asc" })

.. table:: Before

   +----------+---------------------------+---------------+------+-------+
   | Date     | Geo                       | Business      | Plan | Actual|
   +==========+===========================+===============+======+=======+
   | 8/1/2024 | Asia-Pacific              | Energy        | 800  | 850   |
   +----------+---------------------------+---------------+------+-------+
   | 7/1/2024 | Middle East               | Healthcare    | 1200 | 900   |
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
   | 8/1/2024 | Asia-Pacific              | Energy        | 800  | 750   |
   +----------+---------------------------+---------------+------+-------+
   | 9/1/2024 | Asia-Pacific              | Technology    | 1500 | 850   |
   +----------+---------------------------+---------------+------+-------+
   | 7/1/2024 | Middle East               | Healthcare    | 1200 | 900   |
   +----------+---------------------------+---------------+------+-------+
   | 5/1/2024 | Latin America             | Manufacturing | 900  | 1050  |
   +----------+---------------------------+---------------+------+-------+
   | 11/1/2024| Latin America             | Energy        | 2000 | 1800  |
   +----------+---------------------------+---------------+------+-------+