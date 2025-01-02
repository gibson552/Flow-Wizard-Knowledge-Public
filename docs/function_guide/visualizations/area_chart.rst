Area Chart
==========

**Description:**

An Area Chart visual based on the given inputs. It will generate a new tab displaying the chart.

**Function:**

.. code-block:: python

    Area_Chart(table = string, x_axis = string, y_axis = string, title = string)

**Parameters:**

- *Table:* Table name on which to perform the function
- *X Axis:* Column to use for the X axis of the chart
- *Y Axis:* Column to use for the Y axis of the chart
- *Title:* Title for the chart

**Example:**

.. code-block:: python

    Area_Chart(table = Budget, x_axis = "Geo", y_axis = "Actuals", title = "Actuals by Geo")
