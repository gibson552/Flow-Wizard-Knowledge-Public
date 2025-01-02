Math
====

**Description:**

Perform arithmetic upon columns, such as adding two together or executing more complex arithmetic. For math this follows the PEMDAS (Order of Operations). *You remember, the ones you learned back in middle school. ;)* However a few of the mathematical operators may be little different. Look below to see what we use.

**Function:**

.. code-block:: python

    Math(table = string, arith = string, new_col = string)

**Parameters:**

- *Table:* Table name on which to perform function
- *Arithmetic Operation:* Arithmetic operation you wish to perform

  - *addition* | "Actual" + "Plan"
  - *subtraction* | "Actual" - "Plan"
  - *multiplication* | "Actual" * "Plan"
  - *exponentiation* (^) | "Actual" ** "Plan
  - *addition* | +
- *New Column:* Name for the new column

**Example | Simple:**

.. code-block:: python

   Math(table = Budget, arith =  ("Actual"-"Plan")*3, new_col = "Math")

.. table:: Before

   +-------------------+----------------------+---------------+------+---------+
   | Date              | Geo                  | Business      | Plan | Actual  |
   +===================+======================+===============+======+=========+
   | 8/25/2024         | Asia-Pacific         | Energy        | 800  | 750     |
   +-------------------+----------------------+---------------+------+---------+
   | 7/18/2024         | Middle East & A      | Healthcare    | 1200 | 900     |
   +-------------------+----------------------+---------------+------+---------+
   | 5/8/2024          | Latin America        | Manufacturing | 900  | 1050    |
   +-------------------+----------------------+---------------+------+---------+
   | 9/28/2024         | Asia-Pacific         | Technology    | 1500 | 1300    |
   +-------------------+----------------------+---------------+------+---------+
   | 11/13/2024        | Latin America        | Energy        | 2000 | 1800    |
   +-------------------+----------------------+---------------+------+---------+

.. table:: After

   +-------------------+----------------------+---------------+------+---------+------+
   | Date              | Geo                  | Business      | Plan | Actual  | Math |
   +===================+======================+===============+======+=========+======+
   | 8/1/2024          | Asia-Pacific         | Energy        | 800  | 750     | 150  |
   +-------------------+----------------------+---------------+------+---------+------+
   | 7/1/2024          | Middle East & A      | Healthcare    | 1200 | 900     | 900  |
   +-------------------+----------------------+---------------+------+---------+------+
   | 5/1/2024          | Latin America        | Manufacturing | 900  | 900     | 0    |
   +-------------------+----------------------+---------------+------+---------+------+
   | 9/1/2024          | Asia-Pacific         | Technology    | 1500 | 1300    | 600  |
   +-------------------+----------------------+---------------+------+---------+------+
   | 11/1/2024         | Latin America        | Energy        | 2000 | 1800    | 600  |
   +-------------------+----------------------+---------------+------+---------+------+
