---
layout: 		post
title: 			2-Factors authentication
category: 	administration usage
tags:				authentication 
---

<p class="message">
    This page describes how to use 2-Factors authentication from Google.
</p>
<span class="linkmore"></span>

Teampass comes with [2-factors authentication](http://en.wikipedia.org/wiki/Two-step_verification) using Google Authenticator ([to know more](http://en.wikipedia.org/wiki/Google_Authenticator)). It relies on the usage of a portable device the user will use to get his temporary code. This will grant a more secured authentication of your instance of Teampass.

# Administrator point of view

## How to enable?

In order to be activated on your instance of Tempass, you need to activate it through Administration Settings page.

* ![Example image]({{ site.baseurl }}/assets/images/2factors_admin_1.png)

## Activate for users

For security reasons, the administrators or managers have to send the flash code to the users.
This is performed through the Users management page.

Click the 2-factors authentication icon to generate and send an email to the user including the link to the flash code.

* ![Example image]({{ site.baseurl }}/assets/images/2factors_admin_2.png)

# User point of view

## Install Google Authenticator

The first step for the user is to install on a portable device the application “Google Authenticator” ([Apple](https://itunes.apple.com/us/app/google-authenticator/id388497605) - [Android](https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2)).

## Add the Teampass key

The user receives an email which includes a link to the flash code. THis flash code has to be flashed in order the user to know the one time password.

## Get authenticated under Teampass

Getting authenticated under Teampass requires now to enter the login, personal password and OTP. Follow next steps:

Through Google Authenticator application, the user get his OTP.

* ![Example image]({{ site.baseurl }}/assets/images/2factors_user_1.png)

Get to Teampass home page

Enter your credentials

* ![Example image]({{ site.baseurl }}/assets/images/2factors_user_2.png)

You are now authenticated