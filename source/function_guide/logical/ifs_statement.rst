If(s) Statement
===============

**Description:**

An If(s) statement that will perform logical checks on a data table and create a new column based on the specified conditions.

**Function:**

.. code-block:: python

    Ifs(table = string, new_col = string, if_statement = string)

**Parameters:**

- *Table:* Table name on which to perform the function
- *New Column Name:* The name for the new column that will store the result of the If(s) statement
- *Ifs Statement:* The logical statement to evaluate, where column names are formatted as `['column name']`

**Example:**

.. code-block:: python

    Ifs(table = Budget5567, new_col = "Updated Stage",
        if_statement = """
        if ['Stage'] == 'Closed Won':
            return 'Won'
        if ['Stage'] == 'Lost':
            return 'Lost'
        else:
            return 'Do not care'
        """)
