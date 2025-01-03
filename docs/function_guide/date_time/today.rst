Today
====

**Description:**

Creates a column that will be updated based on today's date.

**Function:**

.. code-block:: python

    Today(table = string, new_col = string)

**Parameters:**

- *Table:* Table name on which to perform the function
- *New Column Name:* Name for the new column that will store today's date

**Example:**

.. code-block:: python

    Today(table = Budget, new_col = "Today")

.. table:: Before

   +---------------------+--------------------------------------+------+---------+
   | Date                | Geo - BU                             | Plan | Actual  |
   +=====================+======================================+======+=========+
   | 8/22/2024 16:14:14  | Middle East & Africa - Healthcare    | 1200 | 900     |
   +---------------------+--------------------------------------+------+---------+
   | 8/31/2024 14:33:44  | Middle East & Africa - Energy        | 1150 | 1000    |
   +---------------------+--------------------------------------+------+---------+
   | 8/31/2024 14:03:34  | Latin America - Energy               | 2000 | 1800    |
   +---------------------+--------------------------------------+------+---------+
   | 2/22/2024 7:55:59   | Latin America - Energy               | 1850 | 2000    |
   +---------------------+--------------------------------------+------+---------+
   | 7/3/2024 6:24:57    | Latin America - Energy               | 900  | 900     |
   +---------------------+--------------------------------------+------+---------+
   | 7/16/2024 2:47:47   | Latin America - Energy               | 1050 | 1100    |
   +---------------------+--------------------------------------+------+---------+
   | 10/8/2024 2:50:50   | Asia-Pacific - Energy                | 1500 | 1300    |
   +---------------------+--------------------------------------+------+---------+
   | 6/20/2024 9:45:30   | Asia-Pacific - Energy                | 1700 | 1400    |
   +---------------------+--------------------------------------+------+---------+
   | 8/23/2024 8:48:38   | Asia-Pacific - Technology            | 800  | 750     |
   +---------------------+--------------------------------------+------+---------+
   | 8/2/2024 18:18:18   | Asia-Pacific - Technology            | 950  | 1050    |
   +---------------------+--------------------------------------+------+---------+

.. table:: After

   +---------------------+--------------------------------------+------+--------+------------+
   | Date                | Geo - BU                             | Plan | Actual | Today      |
   +=====================+======================================+======+========+============+
   | 8/22/2024 16:14:14  | Middle East & Africa - Healthcare    | 1200 | 900    | 12/13/2024 |
   +---------------------+--------------------------------------+------+--------+------------+
   | 9/1/2024 12:34:44   | Middle East & Africa - Energy        | 1150 | 1000   | 12/13/2024 |
   +---------------------+--------------------------------------+------+--------+------------+
   | 8/31/2024 14:03:34  | Latin America - Energy               | 2000 | 1800   | 12/13/2024 |
   +---------------------+--------------------------------------+------+--------+------------+
   | 2/22/2024 7:05:05   | Latin America - Energy               | 1850 | 2000   | 12/13/2024 |
   +---------------------+--------------------------------------+------+--------+------------+
   | 2/5/2024 6:59:59    | Latin America - Energy               | 900  | 900    | 12/13/2024 |
   +---------------------+--------------------------------------+------+--------+------------+
   | 7/26/2024 22:47:47  | Latin America - Energy               | 1050 | 1100   | 12/13/2024 |
   +---------------------+--------------------------------------+------+--------+------------+
   | 10/8/2024 22:50:50  | Asia-Pacific - Energy                | 1500 | 1300   | 12/13/2024 |
   +---------------------+--------------------------------------+------+--------+------------+
   | 6/20/2024 9:45:30   | Asia-Pacific - Energy                | 1700 | 1400   | 12/13/2024 |
   +---------------------+--------------------------------------+------+--------+------------+
   | 9/23/2024 8:38:38   | Asia-Pacific - Technology            | 800  | 750    | 12/13/2024 |
   +---------------------+--------------------------------------+------+--------+------------+
   | 8/2/2024 18:18:18   | Asia-Pacific - Technology            | 950  | 1050   | 12/13/2024 |
   +---------------------+--------------------------------------+------+--------+------------+
