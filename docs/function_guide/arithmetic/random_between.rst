Random Between
==============

**Description:**

Returns a random integer between two specified values.

**Function:**

.. code-block:: python

    Random_Between(Table = string, low = string, high = string, new_col = string)

**Parameters:**

- *Table:* Table name on which to perform function
- *Low:* Lowest integer
- *High:* Highest integer
- *New Column Name:* Name for new column

**Example:**

.. code-block:: python

   GroupBy(table = Budget, cols = ["Geo", "Business Unit"], agg_group = {value = "Actual", method = "sum"}, new_table_name = "Sum")

.. table:: Before

   +-------------------+----------------------+---------------+------+---------+
   | Date              | Geo                  | Business      | Plan | Actual  |
   +===================+======================+===============+======+=========+
   | 5/1/2024          | Latin America        | Energy        | 900  | 900     |
   +-------------------+----------------------+---------------+------+---------+
   | 5/1/2024          | Latin America        | Manufacturing | 1050 | 1100    |
   +-------------------+----------------------+---------------+------+---------+
   | 6/1/2024          | Latin America        | Energy        | 1850 | 2000    |
   +-------------------+----------------------+---------------+------+---------+
   | 7/1/2024          | Middle East & Africa | Healthcare    | 1150 | 1000    |
   +-------------------+----------------------+---------------+------+---------+
   | 8/1/2024          | Asia-Pacific         | Energy        | 850  | 750     |
   +-------------------+----------------------+---------------+------+---------+
   | 8/1/2024          | Asia-Pacific         | Technology    | 950  | 1050    |
   +-------------------+----------------------+---------------+------+---------+
   | 9/1/2024          | Asia-Pacific         | Technology    | 1500 | 1300    |
   +-------------------+----------------------+---------------+------+---------+
   | 9/1/2024          | Asia-Pacific         | Energy        | 1700 | 1400    |
   +-------------------+----------------------+---------------+------+---------+

.. table:: After

   +----------------------+---------------+-------------+
   | Geo                  | Business      | Actual_sum  |
   +======================+===============+=============+
   | Latin America        | Energy        | 2900        |
   +----------------------+---------------+-------------+
   | Latin America        | Manufacturing | 2900        |
   +----------------------+---------------+-------------+
   | Middle East & Africa | Healthcare    | 1900        |
   +----------------------+---------------+-------------+
   | Asia-Pacific         | Energy        | 2150        |
   +----------------------+---------------+-------------+
   | Asia-Pacific         | Technology    | 2350        |
   +----------------------+---------------+-------------+