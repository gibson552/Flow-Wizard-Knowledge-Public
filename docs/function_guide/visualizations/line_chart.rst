Line Chart
==========

**Description:**

A Line Chart visual based on the given inputs. It will generate a new tab displaying the chart.

**Function:**

.. code-block:: python

    Line_Chart(table = string, x_axis = string, y_axis = string, title = string)

**Parameters:**

- *Table:* Table name on which to perform the function
- *X Axis:* Column to use for the X axis of the chart
- *Y Axis:* Column to use for the Y axis of the chart
- *Title:* Title for the chart

**Example:**

.. code-block:: python

    Line_Chart(table = Budget, x_axis = "Date", y_axis = "Revenue", title = "Line Chart")

.. table:: Before

   +------------+------+--------+
   | Date       | Geo  | Revenue|
   +============+======+========+
   | 6/1/2024   | USA  | 1200   |
   +------------+------+--------+
   | 7/1/2024   | USA  | 800    |
   +------------+------+--------+
   | 8/1/2024   | USA  | 950    |
   +------------+------+--------+
   | 9/1/2024   | USA  | 1000   |
   +------------+------+--------+
   | 10/1/2024  | USA  | 900    |
   +------------+------+--------+
   | 11/1/2024  | USA  | 1000   |
   +------------+------+--------+
   | 12/1/2024  | USA  | 1500   |
   +------------+------+--------+


.. image:: C:\\Users\\pajjo\\Desktop\\Flow-Wizard-Knowledge\\source\\function_guide\\visualizations\\images\\line_chart.png
   :width: 600px
   :alt: After