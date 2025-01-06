Quickbooks
==========

**Description:**

Connect Quickbooks to Flow Wizard.


**Steps to Connecting:**

- *Step 1:* Select Quickbooks from the import screen, and then click *Next* in the bottom right.

.. image:: ./images/Quickbooks/step_1.png
   :width: 600px
   :alt: After


- *Step 2:* Connect to a Quickbooks  *New Connection:*

  - Step 2a: Select the *New Connection* button
  - Step 2b:
     - *Connection Type:* Select the the Connection type *Quickbooks_OAuth*
     - *Connection Name:* Pick a name for your new connection

.. image:: ./images/Quickbooks/step_2.png
   :width: 600px
   :alt: After
.

- Step 3: Click *External Link to Connect Account* and sign into your Quickbooks account
    - This will re-direct you to a Web Browser to complete the Connection
    - Upon completion the Browser will return a message *"Oauth Code Captured. You can now close this screen"*
    - After this return to Flow Wizard and you will see an *Account Connected* screen

.. image:: ./images/Quickbooks/step_3.png
   :width: 600px
   :alt: After
.

- Step 4: Fill out the necessary information:
   - *Report Name:* The Quickbooks Object to connect to (ie. Balance Sheet, Transaction List, Profit and Loss Detail...)
   - *Report Period:* Select the time period for the report (ie. Today, this Month, This Week-to-Date...)
   - *Pull this report with lookback:* Checkbox for if you would like to pull the same report over several periods
   - *Number of Months to look back:* (Only for Pull this report with lookback = True) Number of periods to look back.
   - *New Table Name:* The name for table to be created from the connection
   - *Skip Rows:* How many rows to be skipped on the file. This can be used if your file has blank rows or un-necessary rows at the top.
   - *Number of Rows:* How many rows you would like to be imported

.. image:: ./images/Quickbooks/step_4.png
   :width: 600px
   :alt: After





