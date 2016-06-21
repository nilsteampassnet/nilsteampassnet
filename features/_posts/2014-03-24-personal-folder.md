---
layout:     post
title:      Personal Folder
categories: feature  
tags:       personal feature security user-guide administration
comments:   true
---

This page introduces Personal Folder feature

## Introduction

Personal Folder is a feature that permit each user to have a kind of personal sand box. 
The idea is to permit the user to store his own Items in an independent context than the rest of the Items.

Personal Items are not encrypted with the Teampass Saltkey. Indeed, the encryption protocol relies on the Personal Saltkey that each user has to define.
This way no decryption is possible by anyone else than the user himself.


## Administration

### Enabling Personal Folder feature

Personal Folder is disabled by default. 

In order to be activated for the Users, an Administrator needs to enable the feature through the Teampass Settings page.

* ![Personal folder administration]({{ site.url }}/img/posts/pf_1.png)

### Storing Personal Saltkey in cookie

Personal Saltkey can be stored in a cookie for more convenience. This will prevent the user to enter it each time he logs in.

This feature needs to be enabled through the Teampass Settings page.

![Personal folder administration]({{ site.url }}/img/posts/pf_2.png)

## Personal Saltkey

Each user defines his own Personal Saltkey that will be used for Personal Items encryption.

<span class="fa fa-warning"></span>&nbsp;If the user looses his saltkey then the Personal Items will not be recoverable!

### Defining a Personal Saltkey

Using the top righ menu button, select "Set Personal Saltkey".

![Personal folder administration]({{ site.url }}/img/posts/pf_10.png)

Then enter the saltkey you want to use.

![Personal folder administration]({{ site.url }}/img/posts/pf_11.png)

Notes:

* Is not mandatory if the user doesn't want to use his Personal Items during this session.
* If not set, when opening the Personal Folder, a warning message will be displayed.

### Changing the Personal Saltkey

The user can change his Personal Saltkey by opening his Profile dialogbox.

![Personal folder administration]({{ site.url }}/img/posts/pf_12.png)

Then in the menu, select "Change my Personal Saltkey"

![Personal folder administration]({{ site.url }}/img/posts/pf_13.png)

And set the new Saltkey

![Personal folder administration]({{ site.url }}/img/posts/pf_14.png)

Click `Change button`. 

<span class="fa fa-info"></span>&nbsp;This will require some time because all existing Personal Passwords need to be re-encrypted with new Saltkey.

### Personal Saltkey is lost

This is the worst case because no recovery is possible. All your passwords are lost.
From the previous Profile dialogbox, click on action "Reset my Personal Saltkey".

![Personal folder administration]({{ site.url }}/img/posts/pf_15.png)

Enter new Saltkey, and click `Change button`. 

<span class="fa fa-info"></span>&nbsp;This will require some time because all existing Personal Passwords need to be re-encrypted with new Saltkey.

## Limitation

Personal Item cannot be shared with any other user.
