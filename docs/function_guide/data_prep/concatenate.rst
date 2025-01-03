Concatenate
========

**Description:**

Combine the data from 2 or more columns together as a string

**Function:**

.. code-block:: python

    Concatenate(table = string, cols = list, new_col = string)

**Parameters:**

- *Table:* Table name on which to perform function
- *Append Table:* Table to append to the parameter Table
- *New Column Name:* Name for new column

**Example:**

.. code-block:: python

   Back_Fill_Blanks(table = df, cols = ["Delta"])

.. table:: Before

   +-------------------+----------------------+---------------+------+---------+-------+
   | Date              | Geo                  | Business      | Plan | Actual  | Delta |
   +===================+======================+===============+======+=========+=======+
   | 5/1/2024          | Latin America        | Energy        | 900  | 900     |       |
   +-------------------+----------------------+---------------+------+---------+-------+
   | 5/1/2024          | Latin America        | Manufacturing | 1050 | 1100    |       |
   +-------------------+----------------------+---------------+------+---------+-------+
   | 6/1/2024          | Latin America        | Energy        | 1850 | 2000    |       |
   +-------------------+----------------------+---------------+------+---------+-------+
   | 6/1/2024          | Latin America        | Manufacturing | 2000 | 1800    |       |
   +-------------------+----------------------+---------------+------+---------+-------+
   | 7/1/2024          | Middle East & Africa | Healthcare    | 1200 | 900     | -300  |
   +-------------------+----------------------+---------------+------+---------+-------+
   | 7/1/2024          | Middle East & Africa | Energy        | 1150 | 1000    | -150  |
   +-------------------+----------------------+---------------+------+---------+-------+
   | 8/1/2024          | Asia-Pacific         | Energy        | 800  | 750     | -50   |
   +-------------------+----------------------+---------------+------+---------+-------+
   | 8/1/2024          | Asia-Pacific         | Technology    | 950  | 1050    | 100   |
   +-------------------+----------------------+---------------+------+---------+-------+
   | 9/1/2024          | Asia-Pacific         | Technology    | 1500 | 1300    | -200  |
   +-------------------+----------------------+---------------+------+---------+-------+
   | 9/1/2024          | Asia-Pacific         | Energy        | 1700 | 1400    | -300  |
   +-------------------+----------------------+---------------+------+---------+-------+

.. table:: After

   +-------------------+----------------------+---------------+------+---------+-------+
   | Date              | Geo                  | Business      | Plan | Actual  | Delta |
   +===================+======================+===============+======+=========+=======+
   | 5/1/2024          | Latin America        | Energy        | 900  | 900     | -300  |
   +-------------------+----------------------+---------------+------+---------+-------+
   | 5/1/2024          | Latin America        | Manufacturing | 1050 | 1100    | -300  |
   +-------------------+----------------------+---------------+------+---------+-------+
   | 6/1/2024          | Latin America        | Energy        | 1850 | 2000    | -300  |
   +-------------------+----------------------+---------------+------+---------+-------+
   | 6/1/2024          | Latin America        | Manufacturing | 2000 | 1800    | -300  |
   +-------------------+----------------------+---------------+------+---------+-------+
   | 7/1/2024          | Middle East & Africa | Healthcare    | 1200 | 900     | -300  |
   +-------------------+----------------------+---------------+------+---------+-------+
   | 7/1/2024          | Middle East & Africa | Energy        | 1150 | 1000    | -150  |
   +-------------------+----------------------+---------------+------+---------+-------+
   | 8/1/2024          | Asia-Pacific         | Energy        | 800  | 750     | -50   |
   +-------------------+----------------------+---------------+------+---------+-------+
   | 8/1/2024          | Asia-Pacific         | Technology    | 950  | 1050    | 100   |
   +-------------------+----------------------+---------------+------+---------+-------+
   | 9/1/2024          | Asia-Pacific         | Technology    | 1500 | 1300    | -200  |
   +-------------------+----------------------+---------------+------+---------+-------+
   | 9/1/2024          | Asia-Pacific         | Energy        | 1700 | 1400    | -300  |
   +-------------------+----------------------+---------------+------+---------+-------+