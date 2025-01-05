Salesforce
==========

**Description:**

Connect Salesforce to Flow Wizard. You can connect directly to *Salesforce Reports* or to *SOQL Queries*.

::

| Unsure what a SOQL Query is? Check this out: https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm


**Steps to Connecting:**

- *Step 1:* Select Salesforce from the import screen, and then click *Next* in the bottom right.

.. image:: ./images/salesforce/step_1.png
   :width: 400px
   :alt: After

- *Step 2:* *New Connection:*  or *Previously saved connections:*

.. image:: ./images/salesforce/step_2.png
   :width: 400px
   :alt: After

- *Step 3:* Click *External Link to Connect Account* and log into your Salesforce account

.. image:: ./images/salesforce/step_3.png
   :width: 400px
   :alt: After

.. image:: ./images/salesforce/step_3b.png
   :width: 400px
   :alt: After

- *Step 4:* Fill out relevant information

  - *Data Source Location:* Pull data from *Salesforce Report* or *SOQL Query*
  - *Report ID:* (Only for Report Data Source) The report ID from the URL. See screenshot below
  - *SOQL:* (Only for SOQL Query) Input your SOQL Query
  - *New Table Name:* The name for table to be created from the connection
  - *Skip Rows:* How many rows to be skipped on the file. This can be used if your file has blank rows or un-necessary rows at the top.
  - *Number of Rows:* How many rows you would like to be imported

.. image:: ./images/salesforce/step_4.png
   :width: 400px
   :alt:

Report ID

.. image:: ./images/salesforce/step_4b.png
   :width: 400px
   :alt: