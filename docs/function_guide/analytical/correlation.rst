Correlation
==========

**Description:**

Measures the strength and direction of a linear relationship between two variables

**Function:**

.. code-block:: python

    Correlation(table = string, first_col =  string, second_col =  string, new_col =  string)

**Parameters:**

- *Table:* Table name on which to perform function
- *First Column:* The 1st column to correlate
- *Second Column:* The 2nd column to correlate
- *New Column Name:* Name for new column



**Example:**

.. code-block:: python

   Correlation(table = Budget, first_col =  "Date", second_col = "Actual", new_col =  "Correl")

.. table:: Before

   +-------------------+----------------------+---------------+------+---------+
   | Date              | Geo                  | Business      | Plan | Actual |
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

.. table:: After

   +-------------------+----------------------+---------------+------+---------+--------------+-------------+
   | Date              | Geo                  | Business      | Plan | Actual | cor. Pearson | cor. Spear  |
   +===================+======================+===============+======+=========+==============+=============+
   | 8/1/2024          | Asia-Pacific         | Energy        | 800  | 750     | 0.720567041  | 0.65        |
   +-------------------+----------------------+---------------+------+---------+--------------+-------------+
   | 7/1/2024          | Middle East & A      | Healthcare    | 1200 | 900     | 0.720567041  | 0.65        |
   +-------------------+----------------------+---------------+------+---------+--------------+-------------+
   | 5/1/2024          | Latin America        | Manufacturing | 900  | 1050    | 0.720567041  | 0.65        |
   +-------------------+----------------------+---------------+------+---------+--------------+-------------+
   | 9/1/2024          | Asia-Pacific         | Technology    | 1500 | 1300    | 0.720567041  | 0.65        |
   +-------------------+----------------------+---------------+------+---------+--------------+-------------+
   | 11/1/2024         | Latin America        | Energy        | 2000 | 1800    | 0.720567041  | 0.65        |
   +-------------------+----------------------+---------------+------+---------+--------------+-------------+