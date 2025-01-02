Compare Columns
==========

**Description:**

Logic compare over two columns (=,>,<,...)

**Function:**

.. code-block:: python

    Compare_Columns(table = string, first_col = string, second_col = string, comparison_type = string, new_col = string)

**Parameters:**

- *Table:* Table name on which to perform function

- *First Column:* 1st in the compare operation

- *Second Column:* 2nd in the compare operation

- *Comparison Type:* What to compare by (=,<,>,<>,!=,<=,>=)

- *New Column Name:* Name of new column created


**Example:**

.. code-block:: python

   Compare_Columns(table = Budget, first_col = "Plan", second_col = "Actual", comparison_type = "<", new_col = "Act Vs Plan")

.. table:: Before

   +-------------------+----------------------+---------------+------+---------+
   | Date              | Geo                  | Business      | Plan | Actual  |
   +===================+======================+===============+======+=========+
   | 8/25/2024         | Asia-Pacific         | Energy        | 800  | 750     |
   +-------------------+----------------------+---------------+------+---------+
   | 7/18/2024         | Middle East & A      | Healthcare    | 1200 | 900     |
   +-------------------+----------------------+---------------+------+---------+
   | 5/8/2024          | Latin America        | Manufacturing | 900  | 1050    |
   +-------------------+----------------------+---------------+------+---------+
   | 9/28/2024         | Asia-Pacific         | Technology    | 1500 | 1300    |
   +-------------------+----------------------+---------------+------+---------+
   | 11/13/2024        | Latin America        | Energy        | 2000 | 1800    |
   +-------------------+----------------------+---------------+------+---------+

.. table:: After

   +-------------------+----------------------+---------------+------+---------+-------------+
   | Date              | Geo                  | Business      | Plan | Actual  | Act vs Plan |
   +===================+======================+===============+======+=========+=============+
   | 8/25/2024         | Asia-Pacific         | Energy        | 800  | 750     | FALSE       |
   +-------------------+----------------------+---------------+------+---------+-------------+
   | 7/18/2024         | Middle East & A      | Healthcare    | 1200 | 900     | FALSE       |
   +-------------------+----------------------+---------------+------+---------+-------------+
   | 5/8/2024          | Latin America        | Manufacturing | 900  | 1050    | TRUE        |
   +-------------------+----------------------+---------------+------+---------+-------------+
   | 9/28/2024         | Asia-Pacific         | Technology    | 1500 | 1300    | FALSE       |
   +-------------------+----------------------+---------------+------+---------+-------------+
   | 11/13/2024        | Latin America        | Energy        | 2000 | 1800    | FALSE       |
   +-------------------+----------------------+---------------+------+---------+-------------+