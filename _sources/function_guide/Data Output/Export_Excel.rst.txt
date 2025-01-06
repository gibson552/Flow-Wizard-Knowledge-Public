Export to Excel
========

**Description:**

Export a table to an Excel file

**Function:**

.. code-block:: python

   Export_Excel(table = Budget, sheet_name = string, export_type = string, FilePath = string, file_name = string, excel_export = {position = string, headers = checkbox} and ...)

**Parameters:**

- *Export Type:* New Excel File, Modify Existing, Create From Template
- *New File Name:* Give the newly created file a new name (Only for *Create from Template*)
- *File Path:* Enter the filepath of the file you would like to export to *Note: add no \ at the end*
- *File Name:* Name of the file
- *Table:* Name of the Flow Wizard table to be exported
- *Sheet Name:* Name for Sheet. No Spaces Allowed
- *Export Position:* Starting location of Data. Ex "A1"
- *Headers:* Include the table headers? (checkbox True or False)


**Example:**

Creating a new Excel file and outputting 2 tables to their own sheet

.. code-block:: python

   Export_Excel(table = Budget, sheet_name = "2025 Budget", export_type = "New Excel File",
   FilePath = "C:\Your\File\Path", file_name = "Budget",
   excel_export = {position = "A1", headers = True}
   and
   {table = Transposed, sheet_name = "2024 Budget", position = "A1", headers = True })

Outputing to an existing Excel file

.. code-block:: python

   Export_Excel(table = Budget, sheet_name = "2025 Budget", export_type = "Modify Existing",
   FilePath = "C:\Your\File\Path", file_name = "Budget",
   excel_export = {position = "A1", headers = True, table = Budget, sheet_name = "sheet1"} )
