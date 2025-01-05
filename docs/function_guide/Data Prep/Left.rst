Left
========

**Description:**

Substring from beginning of column string

**Function:**

.. code-block:: python

    Left(table = string, col = string, num_chars = integer, new_col = string)

**Parameters:**

- *Table:* Table name on which to perform function
- *Column:* Column to perform left
- *Number of Characters:* Number of Charters to look Left
- *New Column Name:* Name for new column

**Example:**

.. code-block:: python

   Left(table = Budget, col = "Date", num_chars = 3, new_col = "Left")

.. table:: Before

   +----------+--------------------------------------+------+---------+
   | Date     | Geo - BU                             | Plan | Actual  |
   +==========+======================================+======+=========+
   | Jul 2024 | Middle East & Africa - Healthcare    | 1200 | 900     |
   +----------+--------------------------------------+------+---------+
   | Jul 2024 | Middle East & Africa - Energy        | 1150 | 1000    |
   +----------+--------------------------------------+------+---------+
   | Jun 2024 | Latin America - Energy               | 2000 | 1800    |
   +----------+--------------------------------------+------+---------+
   | Jun 2024 | Latin America - Energy               | 1850 | 2000    |
   +----------+--------------------------------------+------+---------+


.. table:: After

   +----------+--------------------------------------+------+---------+-------+
   | Date     | Geo - BU                             | Plan | Actual  | Left  |
   +==========+======================================+======+=========+=======+
   | Jul 2024 | Middle East & Africa - Healthcare    | 1200 | 900     | Jul   |
   +----------+--------------------------------------+------+---------+-------+
   | Jul 2024 | Middle East & Africa - Energy        | 1150 | 1000    | Jul   |
   +----------+--------------------------------------+------+---------+-------+
   | Jun 2024 | Latin America - Energy               | 2000 | 1800    | Jun   |
   +----------+--------------------------------------+------+---------+-------+
   | Jun 2024 | Latin America - Energy               | 1850 | 2000    | Jun   |
   +----------+--------------------------------------+------+---------+-------+
