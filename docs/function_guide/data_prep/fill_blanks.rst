Fill Blanks
========

**Description:**

Replace all blank values with a specified value.

**Function:**

.. code-block:: python

    Fill Blanks(table = string, cols= list, fill = string, dtype = drop down)

**Parameters:**

- *Table:* Table name on which to perform function
- *Column(s):* Column(s) to fill blanks in
- *Fill With:* What to fill the blanks with.
- *Data Type:* What data type to fill the blanks with (string, integer, date)

**Example:**

.. code-block:: python

   Fill_Blanks(table = Budget, cols = ["Actual", "Plan"], fill = "0", dtype = "Integer")

.. table:: Before

   +-------------------+----------------------+---------------+------+---------+
   | Date              | Geo                  | Business      | Plan | Actual  |
   +===================+======================+===============+======+=========+
   | 7/1/2024          | Middle East & Africa | Healthcare    | 1200 | 900     |
   +-------------------+----------------------+---------------+------+---------+
   | 7/1/2024          | Middle East & Africa | Healthcare    | 1150 |         |
   +-------------------+----------------------+---------------+------+---------+
   | 8/1/2024          | Asia-Pacific         | Energy        | 800  |         |
   +-------------------+----------------------+---------------+------+---------+
   | 8/1/2024          | Asia-Pacific         | Technology    | 950  | 1050    |
   +-------------------+----------------------+---------------+------+---------+
   | 9/1/2024          | Asia-Pacific         | Technology    |      | 1300    |
   +-------------------+----------------------+---------------+------+---------+
   | 9/1/2024          | Asia-Pacific         | Energy        | 1700 | 1400    |
   +-------------------+----------------------+---------------+------+---------+

.. table:: After

   +-------------------+----------------------+---------------+------+---------+
   | Date              | Geo                  | Business      | Plan | Actual  |
   +===================+======================+===============+======+=========+
   | 7/1/2024          | Middle East & Africa | Healthcare    | 1200 | 900     |
   +-------------------+----------------------+---------------+------+---------+
   | 7/1/2024          | Middle East & Africa | Healthcare    | 1150 | 0       |
   +-------------------+----------------------+---------------+------+---------+
   | 8/1/2024          | Asia-Pacific         | Energy        | 800  | 0       |
   +-------------------+----------------------+---------------+------+---------+
   | 8/1/2024          | Asia-Pacific         | Technology    | 950  | 1050    |
   +-------------------+----------------------+---------------+------+---------+
   | 9/1/2024          | Asia-Pacific         | Technology    | 0    | 1300    |
   +-------------------+----------------------+---------------+------+---------+
   | 9/1/2024          | Asia-Pacific         | Energy        | 1700 | 1400    |
   +-------------------+----------------------+---------------+------+---------+