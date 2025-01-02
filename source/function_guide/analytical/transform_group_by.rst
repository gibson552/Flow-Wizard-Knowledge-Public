Transform Group By
=================

**Description:**

Similar to a groupby but returns a column to original dataset.

**Function:**

.. code-block:: python

    TransformGroupBy(table = string, value = string, cols = list, method = drop down, new_col = string)

**Parameters:**

- *Table:* Table name on which to perform function
- *Value:* Column with Values you wish to evaluate
- *Columns to Group:* Columns that you wish to Group
- *Method:* How to aggregate the data (sum, count, mean, min, max, median)
- *New Column Name:* Name for new grouped table

**Example:**

.. code-block:: python

   TransformGroupBy(table = Budget, value = "Actual", cols = ["Geo"], method = "average", new_col = "Transform")

.. table:: Before

   +-------------------+----------------------+---------------+------+---------+
   | Date              | Geo                  | Business      | Plan | Actual  |
   +===================+======================+===============+======+=========+
   | 8/1/2024          | Asia-Pacific         | Energy        | 800  | 750     |
   +-------------------+----------------------+---------------+------+---------+
   | 7/1/2024          | Middle East & A      | Healthcare    | 1200 | 900     |
   +-------------------+----------------------+---------------+------+---------+
   | 5/1/2024          | Latin America        | Manufacturing | 900  | 1050    |
   +-------------------+----------------------+---------------+------+---------+
   | 9/1/2024          | Asia-Pacific         | Technology    | 1500 | 1300    |
   +-------------------+----------------------+---------------+------+---------+
   | 11/1/2024         | Latin America        | Energy        | 2000 | 1800    |
   +-------------------+----------------------+---------------+------+---------+

.. table:: After | Transform *average*

   +-------------------+----------------------+---------------+------+---------+-----------+
   | Date              | Geo                  | Business      | Plan | Actual  | Transform |
   +===================+======================+===============+======+=========+===========+
   | 8/1/2024          | Asia-Pacific         | Energy        | 800  | 750     | 1130      |
   +-------------------+----------------------+---------------+------+---------+-----------+
   | 7/1/2024          | Middle East & A      | Healthcare    | 1200 | 900     | 1130      |
   +-------------------+----------------------+---------------+------+---------+-----------+
   | 5/1/2024          | Latin America        | Manufacturing | 900  | 900     | 1130      |
   +-------------------+----------------------+---------------+------+---------+-----------+
   | 9/1/2024          | Asia-Pacific         | Technology    | 1500 | 1300    | 1130      |
   +-------------------+----------------------+---------------+------+---------+-----------+
   | 11/1/2024         | Latin America        | Energy        | 2000 | 1800    | 1130      |
   +-------------------+----------------------+---------------+------+---------+-----------+