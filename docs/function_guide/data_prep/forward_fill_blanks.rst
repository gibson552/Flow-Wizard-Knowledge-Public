Forward Fill Blanks
========

**Description:**

Forward Propagation of Missing Data

**Function:**

.. code-block:: python

    Forward_Fill_Blanks(table = string, cols = list)

**Parameters:**

- *Table:* Table name on which to perform function
- *Column(s):* Column(s) to forward fill

**Example:**

.. code-block:: python

   Forward_Fill_Blanks(table = Budget, cols = ["Business Unit", "Geo"])

.. table:: Before

   +-------------------+----------------------+---------------+------+---------+
   | Date              | Geo                  | Business      | Plan | Actual  |
   +===================+======================+===============+======+=========+
   | 7/1/2024          | Middle East & Africa | Healthcare    | 1200 | 900     |
   +-------------------+----------------------+---------------+------+---------+
   | 7/1/2024          | Middle East & Africa | Energy        | 1150 | 1000    |
   +-------------------+----------------------+---------------+------+---------+
   | 6/1/2024          | Latin America        | Energy        | 2000 | 1800    |
   +-------------------+----------------------+---------------+------+---------+
   | 6/1/2024          | Latin America        | Energy        | 1850 | 2000    |
   +-------------------+----------------------+---------------+------+---------+
   | 5/1/2024          | Latin America        | Energy        | 900  | 900     |
   +-------------------+----------------------+---------------+------+---------+
   | 5/1/2024          | Latin America        | Energy        | 1050 | 1100    |
   +-------------------+----------------------+---------------+------+---------+
   | 9/1/2024          | Asia-Pacific         |               | 1500 | 1300    |
   +-------------------+----------------------+---------------+------+---------+
   | 9/1/2024          | Asia-Pacific         |               | 1700 | 1400    |
   +-------------------+----------------------+---------------+------+---------+
   | 8/1/2024          | Asia-Pacific         | Technology    | 800  | 750     |
   +-------------------+----------------------+---------------+------+---------+
   | 8/1/2024          |                      | Technology    | 950  | 1050    |
   +-------------------+----------------------+---------------+------+---------+

.. table:: After

   +-------------------+----------------------+---------------+------+---------+
   | Date              | Geo                  | Business      | Plan | Actual  |
   +===================+======================+===============+======+=========+
   | 7/1/2024          | Middle East & Africa | Healthcare    | 1200 | 900     |
   +-------------------+----------------------+---------------+------+---------+
   | 7/1/2024          | Middle East & Africa | Energy        | 1150 | 1000    |
   +-------------------+----------------------+---------------+------+---------+
   | 6/1/2024          | Latin America        | Energy        | 2000 | 1800    |
   +-------------------+----------------------+---------------+------+---------+
   | 6/1/2024          | Latin America        | Energy        | 1850 | 2000    |
   +-------------------+----------------------+---------------+------+---------+
   | 5/1/2024          | Latin America        | Energy        | 900  | 900     |
   +-------------------+----------------------+---------------+------+---------+
   | 5/1/2024          | Latin America        | Energy        | 1050 | 1100    |
   +-------------------+----------------------+---------------+------+---------+
   | 9/1/2024          | Asia-Pacific         | Energy        | 1500 | 1300    |
   +-------------------+----------------------+---------------+------+---------+
   | 9/1/2024          | Asia-Pacific         | Energy        | 1700 | 1400    |
   +-------------------+----------------------+---------------+------+---------+
   | 8/1/2024          | Asia-Pacific         | Technology    | 800  | 750     |
   +-------------------+----------------------+---------------+------+---------+
   | 8/1/2024          | Asia-Pacific         | Technology    | 950  | 1050    |
   +-------------------+----------------------+---------------+------+---------+