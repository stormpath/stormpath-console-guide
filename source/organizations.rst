.. _organizations:

*************
Organizations
*************

The `Organizations page <https://api.stormpath.com/ui2/index.html#/organizations>`__ contains the list of Organizations in your Stormpath Tenant. On this page you can quickly:

- Search for Organizations in the top-right search box
- :ref:`Add new Organizations <organizations-creating>` using the "Create Organization" button
- :ref:`Change the status of one or more Organizations <organizations-changing-status>` to: `Enabled` or `Disabled`
- :ref:`Delete one or more Organizations <organizations-deleting>`
- :ref:`Edit an Organization <Organizations-editing>`

Finding a Organization's URL
================================

To find an Organization's unique URL, first click on its name from the main list of Organizations. It's URL can be found at the top of the Organization's page, in the field marked "HREF".

Clicking on this URL will open your Organization's information in JSON format and display it in your browser.

.. _organizations-creating:

Creating Organizations
========================

To create a new Organization, start by clicking on **Create Organization** in the top right of the main `Organizations page <https://api.stormpath.com/ui2/index.html#/organizations>`__. This will bring up the "Create Organization" dialog.

From here you must enter in a "Name" for your Organization.

You must also enter in a "Name Key". This must be unique across all Organizations within your Stormpath Tenant and must follow `DNS hostname rules <http://www.ietf.org/rfc/rfc0952.txt>`__. That is, it may only consist of: ``a-z``, ``0-9``, and ``-``. It must not start or end with a hyphen. The uniqueness constraint is case insensitive.

You can also optionally enter in a "Description" for the Organization.

After you have completed this, the "Create Organization" dialog will close and you will see your new Organization in the list of Organizations.

.. _organizations-editing:

Editing Organizations
========================

.. _organizations-changing-status:

Enabling & Disabling Organizations
===================================

Bulk
----

.. _organizations-deleting:

Deleting Organizations
========================

Bulk
----

Other Tasks
=============