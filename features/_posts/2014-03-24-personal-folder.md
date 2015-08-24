---
layout:     post
title:      Personal Folder
categories: feature  
tags:       personal feature security user-guide administration
comments:   true
---

<div class="message">
    This page introduces Personal Folder feature
</div>
<span class="linkmore"></span>

# Introduction

Personal Folder is a feature that permit each user to have a kind of personal sand box. 
The idea is to permit the user to store his own Items in an independent context than the rest of the Items.

Personal Items are not encrypted with the Teampass Saltkey. Indeed, the encryption protocol relies on the Personal Saltkey that each user has to define.
This way no decryption is possible by anyone else than the user himself.


# Administration

## Enabling Personal Folder feature

Personal Folder is disabled by default. 

In order to be activated for the Users, an Administrator needs to enable the feature through the Teampass Settings page.

* ![Personal folder administration]({{ site.url }}/assets/images/pf_1.png)

## Storing Personal Saltkey in cookie

Personal Saltkey can be stored in a cookie for more convenience. This will prevent the user to enter it each time he logs in.

This feature needs to be enabled through the Teampass Settings page.

* ![Personal folder administration]({{ site.url }}/assets/images/pf_2.png)

# Personal Saltkey

Each user defines his own Personal Saltkey that will be used for Personal Items encryption.

<i class="fa fa-warning" style="margin-right:10px;"></i> if the user loses his saltkey then the Personal Items will not be recoverable!

## Defining a Personal Saltkey

In the Home page, the user has to write down his Personal Saltkey.

* ![Personal folder administration]({{ site.url }}/assets/images/pf_3.png)

Notes:

* Is not mandatory if the user doesn't want to use his Persoanl Items during this time.
* If not written and opens a Personal Items, then the password will be empty.

## Changing the Personal Saltkey

The user can change his Personal Saltkey using button "Change it" from the Home page.

* ![Personal folder administration]({{ site.url }}/assets/images/pf_6.png)
* ![Personal folder administration]({{ site.url }}/assets/images/pf_7.png)

## Personal Saltkey is lost

This is the worst case because no recovery is possible. All your passwords are lost.
Using button "Lost it" from the Home page permits to reset all the existing passwords.

* ![Personal folder administration]({{ site.url }}/assets/images/pf_4.png)
* ![Personal folder administration]({{ site.url }}/assets/images/pf_5.png)

# Limitation

This feature comes with a certain number of limitations which are:

* <i class="fa-li fa fa-check" style="margin-right:10px;"></i>It is not possible to manage sub-folders in the Personal Folder. It could be an improvement for the future.
* <i class="fa-li fa fa-check" style="margin-right:10px;"></i>Item sharing is not possible.