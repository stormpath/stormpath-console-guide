.. _applications:

************
Applications
************

The `Applications page <https://api.stormpath.com/ui2/index.html#/applications>`__ contains the list of Applications in your Stormpath Tenant. On this page you can quickly:

- Search for Applications in the top-right search box
- Add new Applications using the "Create Application" button (see :ref:`below <applications-creating>`)
- Change the status of an Application to: `Enabled` or `Disabled`
- Delete an Application
- :ref:`Edit an Application <applications-editing>`

Finding an Application's URL
================================

To find an Application's unique URL, first click on its name from the main list of Applications. It's URL can be found at the top of the Application's page, in the field marked "HREF".

Clicking on this URL will open your Application's information in JSON format and display it in your browser.

.. _applications-creating:

Creating Applications
========================

To create a new Application, start by clicking on **Create Application** in the top right of the main `Applications page <https://api.stormpath.com/ui2/index.html#/applications>`__. This will bring up the "Create Application" dialog.

From here you must enter in a "Name" for your Application.

Optionally, you can also:

- Enter in a "Description" for the Application.
- Toggle the status from its default "Enabled" status to "Disabled"
- Enable or disable the automatic creation of a Directory for this Application. If you check "Match Application Name", the Directory's name will be whatever the Application's "Name" is, plus the word "Directory".

After you have completed this, the "Create Application" dialog will close and you will see your new Application in the list of Applications.

.. _applications-editing:

Editing Applications
========================

To edit an Application, first click on its name from the main list of Applications. This will bring you to the Application's page, with the Application's name displayed on the top.

Here you can edit the Application's:

- Name
- Description
- Status (Enabled or Disabled)
- Authorized Callback URIs (for more on this, please see the Directory chapter sections on Social and SAML login)
- Custom Data

On the left-hand side you will see a set of links to various resources associated with this Application, such as Accounts and Groups. For more information about these, see :ref:`applications-othertasks` below.

Adding Custom Data to an Application
------------------------------------

In the "Custom Data" section of the Application page, you will see two tabs: "Editor" and "JSON".

To add a new Custom Data entry, click the `[∨]`. This will open a menu with the different kinds of fields that you can add. Click on the kind that you want, and a dummy entry will be created, into which you can then enter whatever values you like.

Once you are finished, a green "Saved" notification will appear in the top right of the "Editor" section. If you would like to undo your latest entry, simply click on **Revert**.

To see what your Custom Data would look like as JSON, click on the "JSON" tab.

Enabling & Disabling Applications
=================================

All login attempts in Stormpath are made against a specific Application. As a result, if an Application has a "Disabled" status then any login attempts made to that Application will fail.

You can enable or disable Applications either from:

1. The main list of Applications found on the main `Applications page <https://api.stormpath.com/ui2/index.html#/applications>`__, via the drop-down menus in the "Status" column, or
2. On the page for any individual Application, via the "Status" field.

Choosing to Disable an Application will bring up a confirmation dialog.

Deleting Applications
========================

.. warning::

  Deleting an Application permanently and completely erases it and any of its related data from Stormpath.
  We recommend that you disable Applications instead of deleting them if you anticipate that you might use the Application again or if you want to retain its data for historical reference.

Deleting an Application is done from the `Applications page <https://api.stormpath.com/ui2/index.html#/applications>`__. In the "Action" column, click on **Delete**. This will bring up a confirmation dialog. Once you have read the dialog, select the "I Understand" checkbox and then click on **Delete Application**.

Finding Related Resources
================================

Bulk Actions
=============

.. _applications-othertasks:

Other Tasks
===========

.. _applications-accounts:

Managing an Application's Accounts
-----------------------------------

.. _applications-accountstores:

Managing an Application's Account Stores
----------------------------------------

Dragging!

If nothing else, we will need information on all the things you CAN'T do with mirror directories.

.. _applications-oauth:

Managing an Application's OAuth Policy
--------------------------------------

.. _applications-saml:

Managing an Application's SAML Policy
--------------------------------------