Vlookup
========

**Description:**

Combine two tables of data together based on a key

**Function:**

.. code-block:: python

   Vlookup(table = string, lookup_col = string, lookup_table = string, match_on = string, return_cols = list)

**Parameters:**

- *Table:* Table name on which to perform function
- *Lookup Column:* Column to use as the lookup values
- *Table:* Table to Join to the original Table
- *Match Column:* Column to match lookup column with
- *Columns to Return:* Column(s) to return from the lookup table

**Example:**

.. code-block:: python

   Vlookup(table = Company Data, lookup_col = "Company", lookup_table = Revenue, match_on = "Geo", return_cols = ["MRR"])

.. table:: Before *table 1*

   +----------------+------+
   | Company        | MRR  |
   +================+======+
   | QuantumLeap    | 750  |
   +----------------+------+
   | NebulaTech     | 850  |
   +----------------+------+
   | Eclipse Ent.   | 900  |
   +----------------+------+
   | GalacticCorp   | 1050 |
   +----------------+------+
   | Starforge      | 1800 |
   +----------------+------+

.. table:: Before *table 2*

   +----------------+----------------+
   | Company        | Geo            |
   +================+================+
   | QuantumLeap    | United States  |
   +----------------+----------------+
   | NebulaTech     | Asia-Pacific   |
   +----------------+----------------+
   | Eclipse Ent.   | Middle East    |
   +----------------+----------------+
   | GalacticCorp   | Latin America  |
   +----------------+----------------+
   | Starforge      | Latin America  |
   +----------------+----------------+

----------------------------------------------------------------------------------------------

.. table:: After

   +----------------+----------------+------+
   | Company        | Geo            | MRR  |
   +================+================+======+
   | QuantumLeap    | United States  | 750  |
   +----------------+----------------+------+
   | NebulaTech     | Asia-Pacific   | 850  |
   +----------------+----------------+------+
   | Eclipse Ent.   | Middle East    | 900  |
   +----------------+----------------+------+
   | GalacticCorp   | Latin America  | 1050 |
   +----------------+----------------+------+
   | Starforge      | Latin America  | 1800 |
   +----------------+----------------+------+