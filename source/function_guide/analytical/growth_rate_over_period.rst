Growth Rate over Period
================

**Description:**

Returns an incremental growth rate between 2 time periods.

**Function:**

.. code-block:: python

    GrowthRate(table = string, value = string, cols = list, date_col = string, lookback = drop down, new_table_name = string)

**Parameters:**

- *Table:* Table name on which to perform function
- *Value:* Column with Values you wish to evaluate the growth rate
- *Columns:* Columns to group by
- *Lookback:* Period for which to lookback over (Year over Year, Month over Month, Quarter over Quarter, Week over Week, Day over Day)
- *New Table Name:* Name for new table

**Example:**

.. code-block:: python

   GrowthRate(table = Budget, value = "Amount", cols =["entity", "business_unit"], date_col = "expense_date", lookback = "Year over Year", new_table_name = "Growth Rate Table")
