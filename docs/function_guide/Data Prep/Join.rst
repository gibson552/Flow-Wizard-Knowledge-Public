Append
========

**Description:**

Combine two tables of data together based on a key

**Function:**

.. code-block:: python

    Join(table = Budget, join_table = Budget_2, how = "left", left_on = "Concat", right_on = "Concat", new_table_name = "Joined")

**Parameters:**

- *Table:* Table name on which to perform function
- *Join Table:* Table to Join to the original Table
- *How*: Type of join to perform (left, right, inner, outer

  - *left* Retain only the keys present in the left frame, similar to a SQL left outer join. Maintain the original order of the left keys.
  - *right:* Retain only the keys present in the right frame, similar to a SQL right outer join. Maintain the original order of the right keys.
  - *outer:* Combine keys from both frames, similar to a SQL full outer join. Sort the resulting keys in lexicographical order.
  - *inner:* Retain only the keys common to both frames, similar to a SQL inner join. Maintain the original order of the keys from the left frame.

- *Left On:* Key (column name) to match from left table
- *Right On*: Key (column name) to match from right table


**Example:**

.. code-block:: python

       Join(table = Budget, join_table = Budget_2, how = "left", left_on = "Concat", right_on = "Concat", new_table_name = "Joined")

.. table:: Before *Budget*

   +-------------------+-------------------------------+------+
   | Date              | Concat                        | Plan |
   +===================+===============================+======+
   | 7/1/2024          | Middle East & Africa - Health | 1200 |
   +-------------------+-------------------------------+------+
   | 7/1/2024          | Middle East & Africa - Energy | 1150 |
   +-------------------+-------------------------------+------+
   | 6/1/2024          | Latin America - Energy        | 2000 |
   +-------------------+-------------------------------+------+
   | 6/1/2024          | Latin America - Energy        | 1850 |
   +-------------------+-------------------------------+------+
   | 5/1/2024          | Latin America - Energy        | 900  |
   +-------------------+-------------------------------+------+
   | 5/1/2024          | Latin America - Energy        | 1050 |
   +-------------------+-------------------------------+------+
   | 9/1/2024          | Asia-Pacific - Energy         | 1500 |
   +-------------------+-------------------------------+------+
   | 9/1/2024          | Asia-Pacific - Energy         | 1700 |
   +-------------------+-------------------------------+------+
   | 8/1/2024          | Asia-Pacific - Technology     | 800  |
   +-------------------+-------------------------------+------+
   | 8/1/2024          | Asia-Pacific - Technology     | 950  |
   +-------------------+-------------------------------+------+

.. table:: Before *Budget 2*

   +-------------------+-------------------------------+---------+
   | Date              | Concat                        | Actual  |
   +===================+===============================+=========+
   | 7/1/2024          | Middle East & Africa - Health | 900     |
   +-------------------+-------------------------------+---------+
   | 7/1/2024          | Middle East & Africa - Energy | 1000    |
   +-------------------+-------------------------------+---------+
   | 6/1/2024          | Latin America - Energy        | 1800    |
   +-------------------+-------------------------------+---------+
   | 6/1/2024          | Latin America - Energy        | 2000    |
   +-------------------+-------------------------------+---------+
   | 5/1/2024          | Latin America - Energy        | 900     |
   +-------------------+-------------------------------+---------+
   | 5/1/2024          | Latin America - Energy        | 1100    |
   +-------------------+-------------------------------+---------+
   | 9/1/2024          | Asia-Pacific - Energy         | 1300    |
   +-------------------+-------------------------------+---------+
   | 9/1/2024          | Asia-Pacific - Energy         | 1400    |
   +-------------------+-------------------------------+---------+
   | 8/1/2024          | Asia-Pacific - Technology     | 750     |
   +-------------------+-------------------------------+---------+
   | 8/1/2024          | Asia-Pacific - Technology     | 1050    |
   +-------------------+-------------------------------+---------+

-------------------------------------------------------------------------------------------------------------

.. table:: Before

   +-------------------+-------------------------------+------+---------+
   | Date              | Concat                        | Plan | Actual  |
   +===================+===============================+======+=========+
   | 7/1/2024          | Middle East & Africa - Health | 1200 | 900     |
   +-------------------+-------------------------------+------+---------+
   | 7/1/2024          | Middle East & Africa - Energy | 1150 | 1000    |
   +-------------------+-------------------------------+------+---------+
   | 6/1/2024          | Latin America - Energy        | 2000 | 1800    |
   +-------------------+-------------------------------+------+---------+
   | 6/1/2024          | Latin America - Energy        | 1850 | 2000    |
   +-------------------+-------------------------------+------+---------+
   | 5/1/2024          | Latin America - Energy        | 900  | 900     |
   +-------------------+-------------------------------+------+---------+
   | 5/1/2024          | Latin America - Energy        | 1050 | 1100    |
   +-------------------+-------------------------------+------+---------+
   | 9/1/2024          | Asia-Pacific - Energy         | 1500 | 1300    |
   +-------------------+-------------------------------+------+---------+
   | 9/1/2024          | Asia-Pacific - Energy         | 1700 | 1400    |
   +-------------------+-------------------------------+------+---------+
   | 8/1/2024          | Asia-Pacific - Technology     | 800  | 750     |
   +-------------------+-------------------------------+------+---------+
   | 8/1/2024          | Asia-Pacific - Technology     | 950  | 1050    |
   +-------------------+-------------------------------+------+---------+