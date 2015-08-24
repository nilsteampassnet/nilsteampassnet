---
layout:     post
title:      Type of Users
categories: definition
tags:       definition user-guide role
comments:   true
---

<div style="message">
Teampass relies on 3 roles which are Administrator, Manager and User.
</div>
<span class="linkmore"></span>

# Administrator

The Administrator has to set up Teampass to fit the expectations in term of features.
In order to achieve this goal, his role is to:

* Set the expected options
* Manage the [Folders]() (creation, modification and deletion)
* Manage the [Users Group]() (creation, modification and deletion)
* Manage the Users (creation, modification and deletion)

An Administrator can perform any kind of operation in Teampass except working on Items.

The Administrator is often a member of IT team.

Notice that the Administrator has not access to the Items with his "administrator" account.

<i class="fa fa-bell" style="margin-right:10px;"></i>It is possible to allow Administrator to reach Items by changing the variable `$['admin_full_right']` value to FALSE.

# Manager

A Manager in Teampass is a super user that can:

* manage [Folders]() (creation, modification and deletion) associated to the [Users Group]() he has
* manage Users (modification and deletion) on which he is defined as "main administrator"
* of course, deal with Items

A Manager could be a Team leader.

# User

A User is a normal Teampass user which deal with Items the way defined by Administrator and Manager.
