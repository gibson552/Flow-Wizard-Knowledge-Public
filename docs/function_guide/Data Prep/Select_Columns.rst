Select Columns
========

**Description:**

Select specified columns from a table and create a new table

**Function:**

.. code-block:: python

   Select_Columns(table = string, cols = list, new_table_name = string)

**Parameters:**

- *Table:* Table name on which to perform function
- *Columns to Select:* Columns to select for the new table
- *New Table Name:* Name for new table


**Example:**

.. code-block:: python

   Select_Columns(table = Budget, cols = ["Date", "Revenue"], new_table_name = "Select Table")

.. table:: Before

   +----------+---------------+------+---------+
   | Date     | Business      | Geo  | Revenue |
   +==========+===============+======+=========+
   | 1/1/2024 | Energy        | USA  | 951     |
   +----------+---------------+------+---------+
   | 2/1/2024 | Manufacturing | USA  | 801     |
   +----------+---------------+------+---------+
   | 3/1/2024 | Energy        | USA  | 1200    |
   +----------+---------------+------+---------+
   | 4/1/2024 | Manufacturing | USA  | 901     |
   +----------+---------------+------+---------+

.. table:: After

   +----------+---------+
   | Date     | Revenue |
   +==========+=========+
   | 1/1/2024 | 951     |
   +----------+---------+
   | 2/1/2024 | 801     |
   +----------+---------+
   | 3/1/2024 | 1200    |
   +----------+---------+
   | 4/1/2024 | 901     |
   +----------+---------+