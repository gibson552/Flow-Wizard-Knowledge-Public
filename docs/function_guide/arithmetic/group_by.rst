Group By
========

**Description:**

Groups values together based on a chosen method, such as sum, count, average, etc.

**Function:**

.. code-block:: python

    GroupBy(table = string, value = string, cols = list, method = drop down, new_table_name = string)

**Parameters:**

- *Table:* Table name on which to perform function
- *Value:* Column with values you wish to evaluate
- *Columns to Group:* Columns that you wish to group
- *Method:* How to aggregate the data (sum, count, mean, min, max, median)
- *New Table Name:* Name for new grouped table

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