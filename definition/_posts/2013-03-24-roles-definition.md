---
layout:     post
title:      Roles definition
categories: definition
tags:       definition user roles password complexity
comments:   true
---

<div style="message">
Teampass uses Roles of Users in order to ease access rights definition.
</div>
<span class="linkmore"></span>

# Introduction

A Users Role contains a set of Users. It permits to ease the administration of access rights on Folders.
Indeed access rights on Folders are defined by Users Role. 

Notice that a User may be associated to several Users Role.

<i class="fa fa-bell" style="margin-right:10px;"></i>A good practice is to organize the Users Roles by team or groups of interest.

# Example

Let's consider 3 Users (Us1, Us2 and Us3), 2 Folders (Fld1 and Fld2), and 2 Users Role (UG1 and UG2) defined as below:

* UG1 contains Us1, Us2 and Us3. It is associated to Fld2
* UG2 contains Us2. It is associated to Fld1

Based on this assumption, Us2 is the unique user to have access to both Fdl1 and Fld2.

# Who can?

Creation, modification and deletion can only be performed by an Administrator or a Manager.

Notes:

* The Manager will only see the Roles that he is associated to.
* Deleting a User Group will not delete the associated Users.

# User password complexity

A Users Role also defines the minimum complexity level accepted for user passwords definition.

Notice that if a user belongs to several Users Roles, then the most higher complexity level will be set for his password definition.