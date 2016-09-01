***************
Getting Started
***************

This chapter will show you how to get started with some basic tasks in the Stormpath Admin Console. It assumes only that you have already signed-up for Stormpath and are able to login.

Before we start, the following resources are created inside  Stormpath as soon as you register:

**Two Application resources**

- "My Application", which is automatically created for use with our Quickstarts.
- "Stormpath" which is the Application that represents Stormpath within your Tenant. Because it represents Stormpath, it is used to control who can access the Stormpath Admin Console and API.

**A Directory resource**

There is a "Stormpath Administrators" Directory that is mapped to your Stormpath Application resource. Any Accounts added to this Directory will have access to your Stormpath Admin Console and API.

**An Account**

There is one Account resource which is your Account within Stormpath. If you disable or delete this Account, it will no longer be able to access Stormpath.

**One Tenant**

All of these resources exist within a private data space called your Tenant:

.. raw:: html

  <p>
    <img src="https://docs.stormpath.com/rest/product-guide/latest/_images/default_resources.png"/>
  </p>

Now that we know what exists already, you can familiarize yourself with how the Stormpath Admin Console works by creating a few additional resources yourself.

Create An Application
=====================

From `the Home page <https://api.stormpath.com/ui2/index.html#/>`__, click on the "Applications" tab.

The Application resource represents your real-world application that communicates with Stormpath. Usually, you will have as many Application resources as you have applications that are using Stormpath, though the Stormpath data model is extremely flexible.

The `main Applications page <https://api.stormpath.com/ui2/index.html#/>`__ shows you the list view of all of your Applications. From here, click **Create Application**.

This will bring up the "Create Application" dialog. Here you can enter whatever information you want, the only mandatory field is the "Name". Be sure to keep the "Create new Directory" box checked. This means that when we create our Application, we will also create a new Directory to store all of its user Accounts.

When you are done filling out the information, click **Create**.

You will now be back on the main Applications page, and you will see the new Application you created in the list of Applications.

Add Some Groups
===============

Groups have many uses in Stormpath, but the easiest analogy might be to think of them as labels that are applied to Accounts. These labels can indicate many different things.

For example, a Group can be used to model membership in a particular company. This Group is used to model Company A, and every user Account associated with this Group is an employee of Company A.

As another example, a Group can be used to model an Authorization role. So this Group is used to model the Administrator role, and every user Account associated with this Group has the permissions associated with an Administrator user.

Create an Account
=================

Now lets create an account

Add Some Custom Data to the Account
===================================

Now lets add some customData to this account

Create an API Key
=================

Select an SDK/Integration
=========================

Select the SDK/Integration of my choice
and follow the quick start