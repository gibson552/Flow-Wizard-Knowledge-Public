Text to Columns
========

**Description:**

Split up a string into multiple columns

**Function:**

.. code-block:: python

   Text_to_Cols(table = string, col = string, How = string, split_on = string)

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

   Text_to_Cols(table = Budget, col = "Geo", How = "Delimited", split_on = "Comma")

.. table:: Before

   +----------+---------------------------------------+------+-------+
   | Date     | Geo                                   | Plan | Actual|
   +==========+=======================================+======+=======+
   | 8/1/2024 | United States, Energy                 | 800  | 750   |
   +----------+---------------------------------------+------+-------+
   | 9/1/2024 | Asia-Pacific, Technology              | 1500 | 850   |
   +----------+---------------------------------------+------+-------+
   | 7/1/2024 | Middle East & Africa                  | 1200 | 900   |
   +----------+---------------------------------------+------+-------+
   | 5/1/2024 | Latin America, Manufacturing          | 900  | 1050  |
   +----------+---------------------------------------+------+-------+
   | 11/1/2024| Latin America, Energy                 | 2000 | 1800  |
   +----------+---------------------------------------+------+-------+

.. table:: After

   +----------+---------------------------------------+------+-------+-------------------+----------------+
   | Date     | Geo                                   | Plan | Actual| field_0           | field_1        |
   +==========+=======================================+======+=======+===================+================+
   | 8/1/2024 | United States, Energy                 | 800  | 750   | United States     | Energy         |
   +----------+---------------------------------------+------+-------+-------------------+----------------+
   | 9/1/2024 | Asia-Pacific, Technology              | 1500 | 850   | Asia-Pacific      | Technology     |
   +----------+---------------------------------------+------+-------+-------------------+----------------+
   | 7/1/2024 | Middle East & Africa,                 | 1200 | 900   | Middle East & Afr.| Technology     |
   +----------+---------------------------------------+------+-------+-------------------+----------------+
   | 5/1/2024 | Latin America, Manufacturing          | 900  | 1050  | Latin America     | Manufacturing  |
   +----------+---------------------------------------+------+-------+-------------------+----------------+
   | 11/1/2024| Latin America, Energy                 | 2000 | 1800  | Latin America     | Energy         |
   +----------+---------------------------------------+------+-------+-------------------+----------------+