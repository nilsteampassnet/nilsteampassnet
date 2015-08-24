---
layout: 		post
title: 			Managing Roles
category: 		administration usage
tags:			installation folder role
---

<p class="message">
    This page describes how to create, edit, delete and manage Roles versus Folders.
</p>
<span class="linkmore"></span>

# Access to Roles Management page

Access to the `Roles Management` page.

![Folders Icon]({{ site.baseurl }}/assets/images/mng_roles_1.png)

# Creating a new Role

Click the icon `Add a Role`

![Folders Icon]({{ site.baseurl }}/assets/images/mng_roles_2.png)

And fill in the form

![Folders Icon]({{ site.baseurl }}/assets/images/mng_roles_3.png)

About the form:

* The label is the name of the Role.
* The `Required complexity` corresponds to the minimum password complexity level that a User password (that belong to this Role) needs to fulfil.

The new Role is now added to the list.

![Folders Icon]({{ site.baseurl }}/assets/images/mng_roles_4.png)

# Edit a Role

To edit, click the `edition icon` and fill in the form.

![Folders Icon]({{ site.baseurl }}/assets/images/mng_roles_5.png)

# Delete a Role

To delete, click the `edition icon` and Confirm.

![Folders Icon]({{ site.baseurl }}/assets/images/mng_roles_6.png)

<i class="fa fa-bullhorn" style="margin-right:10px;"></i> Users belonging to this Role will need to be associated to another role.

# Using the rights matrix

The rights matrix permits to allow or not the access of Users in a Role to Folders.
The `Red` cell indicates that the Role is not allowed to access the folder. And the `Green` one indicates that the Role has access to.

![Folders Icon]({{ site.baseurl }}/assets/images/mng_roles_7.png)

This matrix is very powerful and visible. As you can see in the previous screen-capture.

# Allow access to all Items

This feature is disabled by default and is unsecure but it may be helpful.

It's aim is to permit the Users of a Role to have the right to edit/modify all Items they have access to.
It will bypass the settings set for each Item.

<i class="fa fa-bullhorn" style="margin-right:10px;"></i> Only activate this for a Role with limited Users.

To activate this, click on the icon as shown in next screen-capture.

![Folders Icon]({{ site.baseurl }}/assets/images/mng_roles_8.png)
