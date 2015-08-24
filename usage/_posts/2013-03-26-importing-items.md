---
layout:     post
title:      Importing items
category:   usage
tags:       import items
comment:    true
---

<div class="message">
This page describes how to import Items into Teampass
</div>
<span class="linkmore"></span>
# Introduction

It is possible to import Items inside Teampass using exchange files. This could permit you to move your existing items to Teampass.

Teampass propose 2 possible importation formats. One is based upon CSV and the other is specific Keepass XML.

# Exchange formats

## CSV solution

CSV format is the simple one to put in place and the most adaptable depending on your current passwords management.

You need to ensure that the list of your Items to be imported are organized following schematic: `Account`,`Login Name`,`Password`,`Web Site`,`Comments`

It is mandatory to use the character quote ( " ) as text encapsulation.

> If a text contains a quote then it is mandatory to double it. 

Example:

```
"Label","Login","Password","Web Site","Comments"
"Generic Bank #1","jdoe","superS3cret","https://www.genericbank.com","Checking accounts, etc"
"Generic Bank #2","jdoe","S3cret with spaces","https://www.genericbank.com","Checking accounts, etc"
"Retailer Chain #1",,"""Secretstartingwithquotes","https://www.bigboxstore.com",
"Retailer Chain #2",,"'Secretstartingwithsinglequote","https://www.bigboxstore.com",
"Retailer Chain #3",,"'Twosinglequotes'","https://www.bigboxstore.com",
"Health Care #1","jdoe","S3cretwithsinglequote'init","https://www.myhealthcare.com","Health care stuff"
"Health Care #2","jdoe","S3cretwithcomma,init","https://www.myhealthcare.com","Health care stuff"
"Health Care #3","jdoe","S3cretwithdoublequote""init","https://www.myhealthcare.com","Health care stuff"
```

If you create your file through Excel, you should have something similar to the next table.

<table>
  <thead>
    <tr>
      <th>Account</th>
      <th>Login Name</th>
      <th>Password</th>
      <th>Web Site</th>
      <th>Comments</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Yahoo</td>
      <td>Alice</td>
      <td>mypass</td>
      <td>mail.yahoo.com</td>
      <td>my emails</td>
    </tr>
    <tr>
      <td>Gmail</td>
      <td>Bob</td>
      <td>pwd</td>
      <td>gmail.com</td>
      <td></td>
    </tr>
  </tbody>
</table>

## Keepass XML solution

This solution is dedicated for people previously using Keepass as Passwords Manager.
It uses the Export feature of Keepass, that generates a specific XML file which contains the attributes that will be imported into Teampass.

# Administration

Importing feature is disabled by default. That means that an Administrator needs to enable the feature through `Settings` page to allow users to import Items inside Teamass.

# How to?

Importing Items is performed from the `Home` page.
