---
layout:     post
title:      Custom Categories and Fields
category:   definition
tags:       fields folders
comments:   true
noToc:      false
---

<div style="message">
Teampass permits you to define custom Categories for Items.
</div>
<span class="linkmore"></span>

# Introduction

A custom category is a container of custom fields. The category is included in the Item form.
It permits you to define your own fields for the Items that the user should fill in when defining an Item.

You can define as many categories and fields you need.

Categories are associated to Folders. This way, you can tune the Categories you want to associate to specific Folders.

Notice that only Administrator can manage custom categories and fields.

# Example

Consider a Folder called "Credit Cards". 
You may want to create a Category called `Credit Cards` including 2 Fields called `PIN` and `Expiration date`.

Based on this, the 2 extra fields will be displayed for each Item stored in the folder `Credit Cards`.

# How to define?

The page [Define Categories](/administration/2013-03-25-defining-customer-category.html) indicates how to define new custom Categories and Fields.

# Information

<ul class="fa-ul">
  <li><i class="fa-li fa fa-check-square"></i>For security purpose, all data written in customer fields are encrypted
  <li><i class="fa-li fa fa-check-square"></i>This feature consumes more SQL queries (around 5 for each field when updating the Item)
  <li><i class="fa-li fa fa-check-square"></i>Notice that this feature may slow down user actions. This is server dependent and should be part of your reflection on how to optimize Teampass in your environment.
</ul>