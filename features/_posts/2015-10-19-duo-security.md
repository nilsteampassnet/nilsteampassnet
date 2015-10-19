---
layout: post
category: feature
tags: "feature usage duo-security"
published: true
---


<div class="message">
    This page introduces the usage of DUOSecurity. Remember that a 2 factor solution is one of the most efficient way to protect your data inside Teampass. I recommand to use this solution.
</div>

## About DUOSecurity

DUOSecurity is a 2 factor authentication tool securizing any kind of tool requiring a usser authentication. It protects every account with ease.

For complete description, you should switch to [DUOSecurity.com](https://www.duosecurity.com/) website.


## How does it work with Teampass?

Once enabled, this feature will require you to synchronize the accounts in Teampass and DUOSecurity. Each Teampass user login needs to have a similar input inside DUOSecurity.

When a Teampass user will require an access to Teampass, DUOSecurity will check if he/she is allowed to access and he/she will need to confirm the access through a dedicated and personal device (check the [authentication methods](https://www.duosecurity.com/product/methods)). If DUOSecurity confirms the legitimity of the user, then Teampass will allow the user to get connected.


## Define a specific application for your Teampass instance

This chapter describes how to create the DUOSecurity application for your Teampass instance.

 * Get connected to your DUOSecurity dashboard
 * Select `Applications` in the menu
 * Click button `Protect an Application`
 * In the list, select `Web SDK` and click `Protect this application`
 * Give a name to this application (example: Teampass)
 * The next settings could be selected:
   * `Username normalization` set to `none`
   * `New user policy` set to `Require Enrollment`
 * Click button `Save changes`
 
 