---
layout: post
title: Type of Users
categories: definition
tags: 
  - definition
  - "user-guide"
  - role
comments: true
published: true
---




<div style="message">
Teampass relies on different roles which are Administrator, Team Manager, Manager, User and Read-Only.
</div>

# Administrator

The Administrator has to set up Teampass to fit the expectations in term of features.
In order to achieve this goal, his role is to:

* Set the expected options
* Manage the [Folders](./2014-04-20-managing-folders) (creation, modification and deletion)
* Manage the [Users Roles](./2014-04-20-managing-roles) (creation, modification and deletion)
* Manage the Users (creation, modification and deletion)

An Administrator can perform any kind of operation in Teampass except working on Items.

The Administrator is often a member of IT team.

Notice that the Administrator has not access to the Items with his "administrator" account.

<i class="fa fa-bell" style="margin-right:10px;"></i>It is possible to allow Administrator to reach Items by changing the variable `$['admin_full_right']` value to FALSE.

# Manager

A Manager in Teampass is a super user that can:

* manage [Folders](./2014-04-20-managing-folders) (creation, modification and deletion) associated to the [Users Group]() he has
* manage Users (modification and deletion) on which he is defined as "administrator"
* deal with Items

A Manager could be a Team leader.

# Team Manager

A Team Manager has the same rights as a Manager plus the ability to manage all existing users in the Database (except the Administrators).

As a consequence, if you define a user as being `Team Manager`, then this user will automatically inherit of `Manager` rights.

# User

A User is a normal Teampass user which deal with Items the way defined by Administrator and Manager.

# Read-Only

A Read-Only user has no ability to create and modify Items. He has access to the Folders and Items as defined by his account but he will never be able to modify anything.