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

The Application resource represents your real-world application that communicates with Stormpath. Usually, you will have as many Application resources as you have applications that are using Stormpath, though the Stormpath data model is extremely flexible.

From `the Home page <https://api.stormpath.com/ui2/index.html#/>`__, click on the "Applications" tab.

..figure::

The `main Applications page <https://api.stormpath.com/ui2/index.html#/>`__ shows you the list view of all of your Applications. From here, click **Create Application**.

..figure::

This will bring up the "Create Application" dialog. Here you can enter whatever information you want, the only mandatory field is the "Name". Be sure to keep the "Create new Directory" box checked. This means that when we create our Application, we will also create a new Directory to store all of its user Accounts.

..figure::

When you are done filling out the information, click **Create**.

You will now be back on the main Applications page, and you will see the new Application you created in the list of Applications.

..figure::

We also indicated that we wanted to create a Directory alongside this Application. There are two ways we can get to this Directory:

1. We can click on the "Directories" tab, where we will see it in the list of Directories.

..figure::

2. We can click on our newly-created Application, and then click on the **Account Stores** link on the left.

..figure::

Here you will see a list of all of the Directories associated with this Application. Any Directory in this list is mapped to this Application, and its users can log in to the Application. If we click on its name, we will be taken to the page for that Directory.

..figure::


Now that we have an Application and a Directory, we can create a Group.

Create an Account
=================

Accounts in Stormpath are used to model anything that requires access to your application. This means that you can create Accounts for your application's users, but also for things like microservices.

From wherever you are, click on the "Accounts" tab at the top.

..figure::

This will bring you to the Accounts list view, where you will see all of the Accounts currently in your Tenant.

On this page, click **Create Account**.

This will bring up the "Create Account" dialog. For "Account Location" select the Directory we made in the previous step. For "First Name" and "Last Name" you can enter whatever you wish, but the email should be one that you control, since an email will be sent to that address inviting them to your Directory.

Once you click **Create** you will be brought back to the Accounts list view and you will see the new Account that you added there.

Now that we have an Application, a Directory, and an Account, we can create a Group for that Account to be associated with.

Add Some Groups
===============

Groups have many uses in Stormpath, but the easiest analogy might be to think of them as labels that are applied to Accounts. These labels can indicate many different things.

For example, a Group can be used to model membership in a particular company. This Group is used to model Company A, and every user Account associated with this Group is an employee of Company A.

As another example, a Group can be used to model an Authorization role. So this Group is used to model the Administrator role, and every user Account associated with this Group has the permissions associated with an Administrator user.

For the purposes of this introduction, you will create a role Group for regular users and add the existing user Account to it.

From wherever you are, click on the "Groups" tab at the top.

..figure::

The `main Groups page <https://api.stormpath.com/ui2/index.html#/>`__ shows you the list view of all of your Groups. From here, click **Create Group**.

..figure::

This will bring up the "Create Group" dialog. First you must indicate which Directory you would like to create this Group inside. Choose the Directory that you created in the last step.

For the name you can enter anything you like, but for our example we will be creating a role Group for regular, non-administrator users. When you are done entering in your information, click **Create**.

..figure::

You will now be back on the main Groups list view, and you will see the new Group that you created.

Add an Account to the Group
===========================

From the Groups view, click on the Group that you just created. From that Group's main page, click on the **Accounts** link on the left hand side.

..figure::

On this page, click on **Add Existing Account**.

..figure::

This will bring up the "Add Existing Accounts" dialog. Here select the Account we created in the previous step and then click **Add Accounts**.

You will now be back on the "Regular User" Group's main page, and you will see the Account that you added in the list of Accounts.

Add Some Custom Data to the Group
===================================

Primary resources in Stormpath, like Applications, Directories, Groups and Accounts, have Custom Data resources associated with them. Custom Data is able to hold arbitrary data in JSON format. A stored value can be a string, boolean, or number value, as well as an array or entire JSON object.

Create an API Key
=================

Select an SDK/Integration
=========================

Select the SDK/Integration of my choice
and follow the quick start