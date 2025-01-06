UnPivot
==========

**Description:**

Unpivot or transpose a pivoted table

Function:

Unpivot(table = string, id_cols = list, unpivot_cols = list, new_table_name = string)


Parameters:

Table: Table name on which to perform function

Columns to use as Identifier Variables(id_cols ): Which columns to unpivot

Unpivot Column(s): Value Columns to unpivot

New Table Name: Name of the new table that will be created

**Examples:**

.. code-block:: python

   Unpivot(table = Budget, id_cols = ["Geo","Segment"],
            unpivot_cols = ["Plan","Actual"], new_table_name = "Bud Unvcadsvaesvasepivot")


**Examples:**

.. code-block:: python

   Unpivot(table = Budget, id_cols = ["Geo","Segment"], unpivot_cols = ["Plan","Actual"], new_table_name = "Bud Unpivot")


**Examples:**

Unpivot(table = Budget, id_cols = ["Geo","Segment"], unpivot_cols = ["Plan","Actual"], new_table_name = "Bud Unpivot")

Unpivot(table = Budget, id_cols = ["Geo","Segment"], unpivot_cols = ["Plan","Actual"], new_table_name = "Bud Unpivot")

Unpivot(table = Budget, id_cols = ["Geo","Segment"], unpivot_cols = ["Plan","Actual"], new_table_name = "Bud Unpivot")

.. code-block:: python

   Unpivot(table = Budget, id_cols = ["Geo","Segment"], unpivot_cols = ["Plan","Actual"], new_table_name = "Bud Unpivot")
