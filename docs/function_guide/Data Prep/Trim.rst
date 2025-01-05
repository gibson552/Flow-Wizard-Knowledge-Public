Trim
========

**Description:**

Remove beginning and ending spaces on a string

**Function:**

.. code-block:: python

   Trim(table = Budget, cols = ["Geo"])

**Parameters:**

- *Table:* Table name on which to perform function
- *New Table Name:* Name for new table



**Example:**

.. code-block:: python

   Trim(table = Budget, cols = ["Geo", "Business Unit"])

.. table:: Before

   +----------+----------------+---------------+------+-------+
   | Date     | Geo            | Business Unit | Plan | Actual|
   +==========+================+===============+======+=======+
   | 8/1/2024 |   United States| Energy        | 800  | 750   |
   +----------+----------------+---------------+------+-------+
   | 9/1/2024 | Asia-Pacific   |   Technology  | 1500 | 850   |
   +----------+----------------+---------------+------+-------+
   | 7/1/2024 | Middle East    |   Technology  | 1200 | 900   |
   +----------+----------------+---------------+------+-------+
   | 5/1/2024 | Latin America  | Manufacturing | 900  | 1050  |
   +----------+----------------+---------------+------+-------+
   | 11/1/2024| Latin America  | Energy        | 2000 | 1800  |
   +----------+----------------+---------------+------+-------+

.. table:: After

   +----------+----------------+---------------+------+-------+
   | Date     | Geo            | Business Unit | Plan | Actual|
   +==========+================+===============+======+=======+
   | 8/1/2024 | United States  | Energy        | 800  | 750   |
   +----------+----------------+---------------+------+-------+
   | 9/1/2024 | Asia-Pacific   | Technology    | 1500 | 850   |
   +----------+----------------+---------------+------+-------+
   | 7/1/2024 | Middle East    | Technology    | 1200 | 900   |
   +----------+----------------+---------------+------+-------+
   | 5/1/2024 | Latin America  | Manufacturing | 900  | 1050  |
   +----------+----------------+---------------+------+-------+
   | 11/1/2024| Latin America  | Energy        | 2000 | 1800  |
   +----------+----------------+---------------+------+-------+