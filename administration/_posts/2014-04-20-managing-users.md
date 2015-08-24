---
layout: 		post
title: 			Managing Users
category: 		administration usage
tags:			installation user manager
---

<p class="message">
    This page describes how to create, edit, delete and manage Users.
</p>
<span class="linkmore"></span>

# Access to Users Management page

Access to the `Users Management` page.

* ![Folders Icon]({{ site.baseurl }}/assets/images/mng_users_1.png)

# Creating a new User

Click the icon `Add a User`

* ![Folders Icon]({{ site.baseurl }}/assets/images/mng_users_2.png)

And fill in the form

* ![Folders Icon]({{ site.baseurl }}/assets/images/mng_users_3.png)

About the form:

* `Name`, `Last name` and `Login` need to be filled in.
* The `Password` is the one the User will need to use to get connected to Teampass.
* `Email` is used to some specific feature of Teampass.
* `User is administrated by` setting is important. By default, Administrators will manage the Users, but you can also decide that this management could be delegated to the Manager of a Role. In this case, select the Role manager.
* Next 3 settings `Is admin`, `Is Manager` and `Is read only` are related the permission of the User inside Teampass. 
* If `Personal folder` is ticked, then the Personal Folder for this User will be created.
* If `Create folder and role for ***` is ticked, then you can imagine what will happen.

The new Role is now added to the list.

* ![Folders Icon]({{ site.baseurl }}/assets/images/mng_users_4.png)

# Edit a User

Editing a User is done by clicking the text. An edition field will be displayed.
Validate the change by clicking the disk icon.

* ![Folders Icon]({{ site.baseurl }}/assets/images/mng_users_5.png)

To edit settings `Managed by`, `Roles`, `Allowed Folders` or `Forbidden Folders`, you need to use the button.

* ![Folders Icon]({{ site.baseurl }}/assets/images/mng_users_6.png)

## Allowed and Forbidden Folders

Each user is associated to Roles. So it means, he/she can access to the Folders defined through the Role.

Nevertheless you can decide to allow this User to access other Folders than the one allowed by the Role.
For this, you need to use setting `Allowed Folders`.

You can also decide to restrict the access to some Folders using the setting `Forbidden Folders`.

<i class="fa fa-bullhorn" style="margin-right:10px;"></i> This should be very rare and for specific case. If it is regularly used, you should think about arranging your Roles.

# Lock and Delete a User

For some reason, you could need to lock a User.
This will prevent the User to get connected to Teampass.

* ![Folders Icon]({{ site.baseurl }}/assets/images/mng_users_7.png)

You can only `delete` a User that has been previously `locked`.

* ![Folders Icon]({{ site.baseurl }}/assets/images/mng_users_8.png)

To `unlock` a locked User, see next screen-capture

* ![Folders Icon]({{ site.baseurl }}/assets/images/mng_users_9.png)

# Change the User level

You can change the User level by using the check-boxes.

* ![Folders Icon]({{ site.baseurl }}/assets/images/mng_users_10.png)

The Users Levels are:

* `Is Admin`: tick (1) to change the User to Administrator
* `Is Manager`: tick (2) to change the User to Manager
* `Is Read Only`: tick (3) to change the User to become Read Only

# Special actions

For each User, you can:

* Allow to `create folders on Root level`
* Change the `Password`
* Change the `Email`
* See the `Log`

