Right
========

**Description:**

Substring from end of column string

**Function:**

.. code-block:: python

    Right(table = string, col = string, num_chars = integer, new_col = string)

**Parameters:**

- *Table:* Table name on which to perform function
- *Column:* Column to perform right
- *Number of Characters:* Number of Charters to look Left
- *New Column Name:* Name for new column

**Example:**

.. code-block:: python

   Right(table = Budget, col = "Date", num_chars = 4, new_col = "Right")

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


.. table:: Before

   +----------+--------------------------------------+------+---------+-------+
   | Date     | Geo - BU                             | Plan | Actual  | Right |
   +==========+======================================+======+=========+=======+
   | Jul 2024 | Middle East & Africa - Healthcare    | 1200 | 900     | 2024  |
   +----------+--------------------------------------+------+---------+-------+
   | Jul 2024 | Middle East & Africa - Energy        | 1150 | 1000    | 2024  |
   +----------+--------------------------------------+------+---------+-------+
   | Jun 2024 | Latin America - Energy               | 2000 | 1800    | 2024  |
   +----------+--------------------------------------+------+---------+-------+
   | Jun 2024 | Latin America - Energy               | 1850 | 2000    | 2024  |
   +----------+--------------------------------------+------+---------+-------+
