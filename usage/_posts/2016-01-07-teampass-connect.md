---
layout: post
title: "Teampass Connect Add-on"
category: usage
tags: addon firefox
published: true
---



**Teampass Connect** is an add-on working with Firefox web-browser.



## Goal

Its goal is to grab the Items existing in your Teampass instance related to the webpage opened in your web-browser, 
and to permit to fill-in the login/password fields inside those web pages.

## Features

The main features of **Teampass Connect** are:
 * Get the couple ```login/password``` related to the open web-page
 * Fill-in the ```login/password``` fields in the web-page
 * Automatically submit the page
 * Secure access to Teampass Server through the API key
 * Usage of local storage to give fast results

## How does it work?

**Teampass Connect** is sending the *web page URL* to your Teampass Server which performs a query to *list the Items* that fits the URL field with the one sent.

This Items list is then displayed and you can decide to fill-in the login/password fields with correct credentials.

## Requirements

 * For security purpose, it is mandatory to use an HTTPS with certified SSL to encrypt the exchanges between the web-browser and Teampass Server. Indeed user password is not encrypted overwise. 
This might not be necessary if you are using Teampass inside your own network (in a company scope for example).
 * It requires API enabled in Teampass Server
 * Users need an API key to get allowed to connect to Teampass Server database

## Installation

**Teampass Connect** for Firefox is available at [Firefox Add-ons Center](https://addons.mozilla.org/en-US/firefox/addon/teampass-connect/).

**Teampass Connect** requires a specific key to be fully operational.
You can request a 7-days evaluation one by contacting me by mail [nils at teampass.net](mailto:nils@teampass.net).

## Important
**Teampass Connect** is not free of use.
Price is not yet defined.

**Teampass Connect** has just being proposed on Mozilla Add-ons Center and is yet not validated or signed. If you want to use it, you will need to change a variable in Firefox.

 * open a tab and write ```àbout:config```
 * search for variable ```xpinstall.signatures.required````and change it to ```false```
 * install now the add-on

## Todo

 * Migrate to Chrome
 * Synchronize login and/or password changes to Teampass Server
