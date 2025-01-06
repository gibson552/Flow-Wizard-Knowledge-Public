Export to Google Sheet
========

**Description:**

Export a table to a Google Sheet. You must be connected to a Google Sheet in Flow Wizard, if you are not go to the *Data Repo* tab and click the *Connect to a Data Source* button. Dont forget to save your flow first!

**Function:**

.. code-block:: python

   Export_Gsheet(connection_uid = string, table = string, WorkbookName = string, SheetName = string, StartLocation = string)

**Parameters:**


- *Connection Name:* Google Sheet Connection Name from Flow Wizard. *Note: You must be connected to Google Sheets for this to work*
- *Table:* Name of the Flow Wizard table to be exported
- *Workbook Name:* Name of the Google Sheet workbook
- *Sheet Name:* Name of the Google Sheet sheet
- *Start Location:* Starting location of where to paste data (ie. A1)


**Example:**

.. code-block:: python

   Export_Gsheet(connection_uid = "my Gsheet Connection", table = Budget,
   WorkbookName = "Budget 2025", SheetName = "Sheet1", StartLocation = "A1")

