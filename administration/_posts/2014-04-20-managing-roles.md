---
layout: 		post
title: 			Managing Groups
category: 		administration
tags:			
- installation
- folder
- role
- - group
---

> This page describes how to create, edit, delete and manage Groups versus Folders.


# Access to Groups Management page

Access to the `Groups Management` page.

![Folders Icon]({{ site.baseurl }}/img/posts/mng_roles_1.png)

# Creating a new Group

Click the icon `Add a Group`

![Folders Icon]({{ site.baseurl }}/img/posts/mng_roles_2.png)

And fill in the form

![Folders Icon]({{ site.baseurl }}/img/posts/mng_roles_3.png)

About the form:

* The label is the name of the Group.
* The `Required complexity` corresponds to the minimum password complexity level that a User password (that belong to this Group) needs to fulfil.

The new Group is now added to the list.

![Folders Icon]({{ site.baseurl }}/img/posts/mng_roles_4.png)

# Edit a Role

To edit, click the `edition icon` and fill in the form.

![Folders Icon]({{ site.baseurl }}/img/posts/mng_roles_5.png)

# Delete a Role

To delete, click the `edition icon` and Confirm.

![Folders Icon]({{ site.baseurl }}/img/posts/mng_roles_6.png)

<span class="fa fa-bullhorn"></span>&nbsp;Users belonging to this Group will need to be associated to another Group.

# Using the Matrix

The Matrix permits to set the expected level of Rights the Group will have on the Folders.

Using the Matrix, click on the cell corresponding to the Group and the Folder you want to change.

A dialogbox will appear in which you can select the type of access rights you want for the Users belonging to this Group on this Folder.

As a consequence, the cell will change color and a specific symbol will indicate the type of allowed rights.

* An open-hand symbol indicates that **no access** is allowed. In such case, the cell is RED.
* An eye symbol indicates that **reading** is allowed. In such case, the cell is ORANGE.
* An indentation symbol indicates that **writing** is allowed.
* A pencil symbol indicates that **editing** is allowed.
* An eraser symbol indicates that **deleting** is allowed.

The cell will be GREEN if rights Write/Edit/Delete are allowed.

The cell will be BLUE if one or two of the rights Write/Edit/Delete are allowed.

![Folders Icon]({{ site.baseurl }}/img/posts/mng_roles_7.png)

This matrix is very powerful and visible. As you can see in the previous screen-capture.

# Allow access to all Items

This feature is disabled by default and is unsecure but it may be helpful.

It's aim is to permit the Users of a Group to have the right to edit/modify all Items they have access to.
It will bypass the settings set for each Item.

<span class="fa fa-bullhorn"></span>&nbsp;Only activate this for a Group with limited Users.

To activate this, click on the icon as shown in next screen-capture.

![Folders Icon]({{ site.baseurl }}/img/posts/mng_roles_8.png)
