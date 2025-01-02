Filter
========

**Description:**

Filter the table by a set of condition(s).

**Function:**

.. code-block:: python

    Filter(table = string, filter_group = {col = string, logical_choice = drop down, filter_value = string} and ...)

**Parameters:**

- *Table:* Table name on which to perform function
- *Column:* Column to filter on a set of condition(s)
- *Logical Choice:* Expression to compare for the filter (Equals, Not Equals, Greater than....)

**Example:**

.. code-block:: python

   Filter(table = Budget, filter_group = {col = "Geo", logical_choice = "Equals", filter_value = "Latin America"} and {col = "Actual", logical_choice = "Greater Than Or Equal", filter_value = "1000" })

.. table:: Before

   +-------------------+----------------------+---------------+------+---------+
   | Date              | Geo                  | Business      | Plan | Actual  |
   +===================+======================+===============+======+=========+
   | 7/1/2024          | Middle East & Africa | Healthcare    | 1200 | 900     |
   +-------------------+----------------------+---------------+------+---------+
   | 7/1/2024          | Middle East & Africa | Healthcare    | 1150 | 1000    |
   +-------------------+----------------------+---------------+------+---------+
   | 6/1/2024          | Latin America        | Manufacturing | 2000 | 1800    |
   +-------------------+----------------------+---------------+------+---------+
   | 6/1/2024          | Latin America        | Energy        | 1850 | 2000    |
   +-------------------+----------------------+---------------+------+---------+
   | 5/1/2024          | Latin America        | Energy        | 900  | 900     |
   +-------------------+----------------------+---------------+------+---------+
   | 5/1/2024          | Latin America        | Manufacturing | 1050 | 1100    |
   +-------------------+----------------------+---------------+------+---------+
   | 9/1/2024          | Latin America        | Manufacturing | 1500 | 1300    |
   +-------------------+----------------------+---------------+------+---------+
   | 9/1/2024          | Asia-Pacific         | Technology    | 1500 | 1300    |
   +-------------------+----------------------+---------------+------+---------+
   | 9/1/2024          | Asia-Pacific         | Energy        | 1700 | 1400    |
   +-------------------+----------------------+---------------+------+---------+
   | 8/1/2024          | Asia-Pacific         | Energy        | 800  | 750     |
   +-------------------+----------------------+---------------+------+---------+
   | 8/1/2024          | Asia-Pacific         | Technology    | 950  | 1050    |
   +-------------------+----------------------+---------------+------+---------+

.. table:: After

   +-------------------+----------------------+---------------+------+---------+
   | Date              | Geo                  | Business      | Plan | Actual  |
   +===================+======================+===============+======+=========+
   | 6/1/2024          | Latin America        | Manufacturing | 2000 | 1800    |
   +-------------------+----------------------+---------------+------+---------+
   | 6/1/2024          | Latin America        | Energy        | 1850 | 2000    |
   +-------------------+----------------------+---------------+------+---------+
   | 5/1/2024          | Latin America        | Manufacturing | 1050 | 1100    |
   +-------------------+----------------------+---------------+------+---------+