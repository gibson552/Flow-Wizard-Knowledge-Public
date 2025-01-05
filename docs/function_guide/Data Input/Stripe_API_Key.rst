Stripe
==========

**Description:**

Connect Stripe to Flow Wizard.
Supported Objects to connect to:
 - Subscriptions
 - Customers
 - Products
 - Quotes
 - Invoices
 - Prices
 - Plans
 - Disputes


**Steps to Connecting:**

- *Step 1:* Select Stripe from the import screen, and then click *Next* in the bottom right.

.. image:: ./images/stripe/step_1.png
   :width: 400px
   :alt: After


---------


- *Step 2:* *New Connection:*  or *Previously saved connections:*

.. image:: ./images/stripe/step_2.png
   :width: 400px
   :alt: After

-------------------------------------------------------------------------------

- *Step 3:* Select Connection Type *Stripe_API_Key* and type a custom name to label you connection in *Connection Name*

.. image:: ./images/stripe/step_3.png
   :width: 400px
   :alt: After


- *Step 4:* Input your Stripe API Key. This can be found on your *Stripe account > Settings > Developers > API keys > Publishable key*. Copy the Publishable key into Flow Wizard to connect.

.. image:: ./images/google_sheets/step_4.png
   :width: 400px
   :alt:

.. image:: ./images/google_sheets/step_4b.png
   :width: 400px
   :alt:

- *Step 5:* Fill out relevant information

  - *Object:* Stripe object you wish to pull data from
  - *New Table Name:* The name for table to be created from the connection
  - *Skip Rows:* How many rows to be skipped on the file. This can be used if your file has blank rows or un-necessary rows at the top.
  - *Number of Rows:* How many rows you would like to be imported


.. image:: ./images/stripe/step_5.png
   :width: 400px
   :alt: