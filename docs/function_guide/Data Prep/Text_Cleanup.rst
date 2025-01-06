Text Cleanup
========

**Description:**

Format text columns in a few ways

**Function:**

.. code-block:: python

   Text_Cleanup(table = Budget, cols = ["Geo", "Business Unit"], l_strip = True, r_strip = True, fill_blank = False, format_text = True, format = "Upper Case")

**Parameters:**

- *Table:* Table name on which to perform function
- *Columns to Clean:* Column(s) to clean up
- *Remove Left leading characters?:* Removes left leading characters
- *Remove Right leading characters?:* Removes right leading characters
- *Fill Blanks?:* Fill in blanks with "Blank"
- *Format Text Case?:* Format the text casing
- *Text Formating:* Format to UPPER CASE, lower case, or Proper Case



**Example:**

.. code-block:: python

   Text_Cleanup(table = Budget, cols = ["Geo", "Business Unit"], l_strip = True, r_strip = True, fill_blank = True, format_text = True, format = "Upper Case")

.. table:: Before

   +----------+---------------------------+---------------+------+-------+
   | Date     | Geo                       | Business      | Plan | Actual|
   +==========+===========================+===============+======+=======+
   | 8/1/2024 |                           | Energy        | 800  | 850   |
   +----------+---------------------------+---------------+------+-------+
   | 7/1/2024 | USA                       | Healthcare    | 1200 | 900   |
   +----------+---------------------------+---------------+------+-------+
   | 5/1/2024 |   Latin America           |               | 900  | 1050  |
   +----------+---------------------------+---------------+------+-------+
   | 9/1/2024 |   Asia-Pacific            | Technology    | 1500 | 750   |
   +----------+---------------------------+---------------+------+-------+
   | 11/1/2024| Latin America             | Energy        | 2000 | 1800  |
   +----------+---------------------------+---------------+------+-------+

.. table:: After

   +----------+---------------------------+---------------+------+-------+
   | Date     | Geo                       | Business      | Plan | Actual|
   +==========+===========================+===============+======+=======+
   | 8/1/2024 | Blank                     | ENERGY        | 800  | 750   |
   +----------+---------------------------+---------------+------+-------+
   | 9/1/2024 | USA                       | HEALTHCARE    | 1500 | 850   |
   +----------+---------------------------+---------------+------+-------+
   | 7/1/2024 | MIDDLE EAST               | Blank         | 1200 | 900   |
   +----------+---------------------------+---------------+------+-------+
   | 5/1/2024 | ASIA-PACIFIC              | TECHNOLOGY    | 900  | 1050  |
   +----------+---------------------------+---------------+------+-------+
   | 11/1/2024| LATIN AMERICA             | ENERGY        | 2000 | 1800  |
   +----------+---------------------------+---------------+------+-------+