HubSpot
==========

**Description:**

Connect HubSpot to Flow Wizard.


**Steps to Connecting:**

- *Step 1:* Select HubSpot from the import screen, and then click *Next* in the bottom right.

.. image:: C:\Users\pajjo\Desktop\Flow-Wizard-Knowledge\source\function_guide\data_input\images\hubspot\step_1.png
   :width: 600px
   :alt: After

-------------------------------------------------------------------------------

- *Step 2:* Connect to a HubSpot *New Connection:*

  - Step 2a: Select the *New Connection* button
  - Step 2b:
     - *Connection Type:* Select the the Connection type *HubSpot OAuth Connection*
     - *Connection Name:* Pick a name for your new connection

.. image:: C:\Users\pajjo\Desktop\Flow-Wizard-Knowledge\source\function_guide\data_input\images\hubspot\step_2a.png
   :width: 600px
   :alt: After
.
  - Step 2c: Click *External Link to Connect Account* and sign into your HubSpot account
     - This will re-direct you to a Web Browser to complete the Connection
     - Upon completion the Browswer will return a message *"Oauth Code Captured. You can now close this screen"*
     - After this return to Flow Wizard and you will see an *Account Connected* screen

.. image:: C:\Users\pajjo\Desktop\Flow-Wizard-Knowledge\source\function_guide\data_input\images\hubspot\step_2c.png
   :width: 600px
   :alt: After
.
  - Step 2d: Fill out the necessary information:
     - *Object:* The HubSpot Object to connect to (ie. Companies, Deals, Contacts...)
     - *New Table Name:* The name for table to be created from the connection
     - *Skip Rows:* How many rows to be skipped on the file. This can be used if your file has blank rows or un-necessary rows at the top.
     - *Number of Rows:* How many rows you would like to be imported
.. image:: C:\Users\pajjo\Desktop\Flow-Wizard-Knowledge\source\function_guide\data_input\images\hubspot\step_2d.png
   :width: 600px
   :alt: After
.



- *Step 2:* Connect to a HubSpot *Previously saved connections:*

.. image:: C:\Users\pajjo\Desktop\Flow-Wizard-Knowledge\source\function_guide\data_input\images\hubspot\step_2b.png
   :width: 600px
   :alt: After

-------------------------------------------------------------------------------

- *Step 3:* Pick a Google Sheets file. Click *Pick File* then in the pop up window search and select the file you wish to connect.

.. image:: C:\Users\pajjo\Desktop\Flow-Wizard-Knowledge\source\function_guide\data_input\images\hubspot\step_3.png
   :width: 600px
   :alt: After

- *Step 4:* Fill out the necessary information:

  - *GSheet File:* This will already be filled out with the Google Sheet ID.
  - *Sheet Name:* The sheet to be connected. Note: this will automatically populate with all available sheet names.
  - *New Table Name:* The name for table to be created from the connection
  - *Skip Rows:* How many rows to be skipped on the file. This can be used if your file has blank rows or un-necessary rows at the top.
  - *Number of Rows:* How many rows you would like to be imported

.. image:: C:\Users\pajjo\Desktop\Flow-Wizard-Knowledge\source\function_guide\data_input\images\hubspot\step_4.png
   :width: 600px
   :alt:

- *Step 5:* Select *Finish* or *Preview*

  - *Finish:* Complete the connection and continue on to build your flow
  - *Preview:* Review your imported table before your finish the connection

.. image:: C:\Users\pajjo\Desktop\Flow-Wizard-Knowledge\source\function_guide\data_input\images\hubspot\step_5.png
   :width: 600px
   :alt:

