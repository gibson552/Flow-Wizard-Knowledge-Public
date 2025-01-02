Rank by Group
==========

**Description:**

Function that ranks values within a specified group

**Function:**

.. code-block:: python

    Rank_by_Group(table = string, value = string, cols = [string], new_col = string, method = string)

**Parameters:**

- *Table:* Table name that you wish to describe

- *Value:* Value by which to rank the group

- *Cols:* Columns to create grouping

- *New_col:* New column name for the ranks to return

+ *Method:* How you want to rank the values (average, min, max, first, dense)

    + average: average rank of group.

    + min: lowest rank in group.

    + max: highest rank in group.

    + first: ranks assigned in order they appear in the array.

    + dense: like "min", but rank always increases by 1 between groups.



**Example:**

.. code-block:: python

   Rank_by_Group(table = Budget, value = "Actual", cols = ["Geo"], method = "average", new_col = "RankbyGroup avg")

.. table:: Before

   +-------------------+----------------------+---------------+------+---------+
   | Date              | Geo                  | Business      | Plan | Actual  |
   +===================+======================+===============+======+=========+
   | 8/1/2024          | Asia-Pacific         | Energy        | 800  | 750     |
   +-------------------+----------------------+---------------+------+---------+
   | 7/1/2024          | Middle East & Africa | Healthcare    | 1200 | 900     |
   +-------------------+----------------------+---------------+------+---------+
   | 5/1/2024          | Latin America        | Manufacturing | 900  | 900     |
   +-------------------+----------------------+---------------+------+---------+
   | 9/1/2024          | Asia-Pacific         | Technology    | 1500 | 1300    |
   +-------------------+----------------------+---------------+------+---------+
   | 11/1/2024         | Latin America        | Energy        | 2000 | 1800    |
   +-------------------+----------------------+---------------+------+---------+

.. table:: Rank by Group *average*

   +-------------------+----------------------+---------------+------+---------+------+
   | Date              | Geo                  | Business      | Plan | Actual  | Avg  |
   +===================+======================+===============+======+=========+======+
   | 8/1/2024          | Asia-Pacific         | Energy        | 800  | 750     | 2    |
   +-------------------+----------------------+---------------+------+---------+------+
   | 7/1/2024          | Middle East & Africa | Healthcare    | 1200 | 900     | 1    |
   +-------------------+----------------------+---------------+------+---------+------+
   | 5/1/2024          | Latin America        | Manufacturing | 900  | 900     | 2    |
   +-------------------+----------------------+---------------+------+---------+------+
   | 9/1/2024          | Asia-Pacific         | Technology    | 1500 | 1300    | 1    |
   +-------------------+----------------------+---------------+------+---------+------+
   | 11/1/2024         | Latin America        | Energy        | 2000 | 1800    | 1    |
   +-------------------+----------------------+---------------+------+---------+------+

