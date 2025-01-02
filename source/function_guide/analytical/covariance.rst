Covariance
==========

**Description:**

Measures the degree to which two variables change together. A positive covariance indicates that the variables tend to increase together, while a negative covariance means that when one increases, the other tends to decrease.

**Function:**

.. code-block:: python

    Covariance(table = string, first_col =  string, second_col =  string, new_col =  string)

**Parameters:**

- *Table:* Table name on which to perform function
- *First Column:* The 1st column to calculate the covariance
- *Second Column:* The 2nd column to calculate the covariance
- *New Column Name:* Name for new column

**Example:**

.. code-block:: python

   Covariance(table = Budget, first_col =  "Date", second_col = "Actual", new_col =  "Covariance"

.. table:: Before

   +-------------------+----------------------+---------------+------+---------+
   | Date              | Geo                  | Business      | Plan | Actual  |
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

   +-------------------+----------------------+---------------+------+---------+-------------+
   | Date              | Geo                  | Business      | Plan | Actuals | Covariance  |
   +===================+======================+===============+======+=========+=============+
   | 8/1/2024          | Asia-Pacific         | Energy        | 800  | 750     | 16280       |
   +-------------------+----------------------+---------------+------+---------+-------------+
   | 7/1/2024          | Middle East & A      | Healthcare    | 1200 | 900     | 16280       |
   +-------------------+----------------------+---------------+------+---------+-------------+
   | 5/1/2024          | Latin America        | Manufacturing | 900  | 1050    | 16280       |
   +-------------------+----------------------+---------------+------+---------+-------------+
   | 9/1/2024          | Asia-Pacific         | Technology    | 1500 | 1300    | 16280       |
   +-------------------+----------------------+---------------+------+---------+-------------+
   | 11/1/2024         | Latin America        | Energy        | 2000 | 1800    | 16280       |
   +-------------------+----------------------+---------------+------+---------+-------------+