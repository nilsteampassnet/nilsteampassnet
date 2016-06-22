---
layout: post
title: Group definition
categories: definition
tags: 
  - definition
  - user
  - group
comments: true
published: true
---


Teampass uses Groups of Users in order to ease access rights definition.

## Definition

A Group contains the access rights setup on Folders. As a consequence, when a User is allocated to a Group, this User inherits of the the Folders access rights as defined for this Group. 

It permits to ease the administration of access rights on Folders.

Notice that a User may be associated to several Groups.

<span class="fa fa-bulb"></span>&nbsp;A good practice is to organize the Groups by team or group of interest.

### Example

Let's consider 3 Users (Us1, Us2 and Us3), 2 Folders (Fld1 and Fld2), and 2 Groups (G1 and G2) defined as below:

* G1 allow access to Fld2
* G2 allow access to Fld1
* Us1, Us2 and Us3 are allocated to G1
* Us2 is allocated to G2

Based on this, Us2 is the unique user to have access to both Fdl1 and Fld2.

### Create, modify and delete

Creation, modification and deletion can only be performed by an **Administrator** or a **Manager**.

Notes:

* The Manager will only see the Groups that he is associated to.
* Deleting a Group will not delete allocated Users.

## Access rights on Folders

A Group permits to define the access rights of allocated Users on the Folders.

The possible access rights of a Group on a Folder are:

* No Access
* Read-Only
* Write
	* with no restriction in edition and/or deletion
	* with no Items edition rights
	* with no Items deletion rights

Based upon those different rights, it is possible to build fine tunned configuration for Users access on Folders.