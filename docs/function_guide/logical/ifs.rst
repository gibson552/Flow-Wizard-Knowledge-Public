IFs
===

**Description:**

Make logical comparisons between a value and what you expect. This function allows for complex logical evaluations where multiple conditions can be chained together.

**Function:**

.. code-block:: python

    Ifs(table = string, if_statement = {if = {col = string, logical_choice = string, value = string}, then = string}, else_value = string, new_col = string)

**Parameters:**

- *Table:* Table name on which to perform the function
- *Ifs Statement:* Logical statement to evaluate, can contain multiple conditions
    - *Column:* The column to evaluate
    - *Logical Selection:* The method to evaluate the column (e.g., "Equals", "Greater than", "Is before date")
    - *Value:* The value to compare in the column based on the logical selection (e.g., X = Y)
    - *Then:* The value to return if the condition is met
    - *Else:* The value to return if none of the conditions are met
- *New Column Name:* The name for the new column that will store the result of the logical evaluation

**Example:**

.. code-block:: python

    Ifs(table = Budget,
        if_statement = {
            if = {col = "Geo", logical_choice = "Equals", value = "USA", if_group_logic = "And", col = "Segment", logical_choice = "Equals", value = "Mid Market"},
            then = "USA MM"
        },
        else_value = "Small Business",
        new_col = "Ifs statement")
