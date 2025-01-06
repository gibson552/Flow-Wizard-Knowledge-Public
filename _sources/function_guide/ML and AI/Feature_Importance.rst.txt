Feature Importance
====

**Description:**

Machine Learning Time Series model to predict future values. This can be based on daily, monthly, or hourly values.

**Function:**

.. code-block:: python

    Feature_Importance(table = string, value_col = string, measure_cols = list,
    n_estimators = integer, random_state = integer, new_table_name = string)

**Parameters:**

- *Table:* Table name on which to perform the function
- *Value Column:* Column to measure the feature importance on
- *Measure Columns:* Columns test feature importance
- *Number of Estimators:* Number of trees: more trees can be more accurate but take longer (pick a number between 10 & 500)
- *Random State:* Random seed: this will allow you to replicate the model (pick a number between 1 & 100)
- *New Table Name:* Name for the new table

**Example:**

.. code-block:: python

    Feature_Importance(table = Budget, value_col = "Revenue", measure_cols = ["Business Unit", "Employee Size", "Geo"],
    n_estimators = 42, random_state = 99, new_table_name = "Feature Imp." )


