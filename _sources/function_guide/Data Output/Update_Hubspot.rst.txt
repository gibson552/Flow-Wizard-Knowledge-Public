Update HubSpot
========

**Description:**

Update Records in Hubspot. You must be connected to a HubSpot in Flow Wizard, if you are not go to the *Data Repo* tab and click the *Connect to a Data Source* button. Dont forget to save your flow first!

**Function:**

.. code-block:: python

   Update_Hubspot(connection_uid = string, object = string, table = string)

**Parameters:**

- *Connection Name:* Google Sheet Connection Name from Flow Wizard. *Note: You must be connected to HubSpot in Flow Wizard for this to work*
- *Object:* Name of the HubSpot Object to send the Flow Wizard table (ie. Companies, Contacts, Deals, ect...)
- *Table:* Name of the Flow Wizard table to be exported

**Example:**

.. code-block:: python

   Update_Hubspot(connection_uid = "my HubSpot connection", object = "Deals", table = DealsClean)
