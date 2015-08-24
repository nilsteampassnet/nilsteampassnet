---
layout: 		post
title: 			Suggestion system
category:		feature
tags:			feature suggestion read-only item
---

<p class="message">
    This page describes the items Suggestion System.
</p>
<span class="linkmore"></span>

# Introduction

The goal of Suggestion System is to provide the ability to Read-Only users to suggest new Items or modification of existing Items.

# Administration - Enabling Suggestion System feature

Suggestion System is disabled by default. 

In order to be activated it, an Administrator needs to enable the feature through the Teampass Settings page.

* ![Personal folder administration]({{ site.url }}/assets/images/suggestion_system_1.png)

# Description

As shown in next screen-capture, accessing to Suggestion System page is done using a specific Icon in the top menu bar.

* ![Personal folder administration]({{ site.url }}/assets/images/suggestion_system_2.png)

This Icon is only available for `Read-Only`, `Manager` and `Administrator` users.

# Main page

It is a classical table view that permits to quickly identify the existing suggestion and to create new suggestions.

* ![Personal folder administration]({{ site.url }}/assets/images/suggestion_system_3.png)

# Adding a Suggestion

## How to?

New Suggestion is done using the `Add Button`.
The Suggestion definition is done through the next form.

* ![Personal folder administration]({{ site.url }}/assets/images/suggestion_system_4.png)

The next fields are used:

* `Label` is the Item label
* `Description` is the Item Description
* `Folder` indicates in what folder the Suggestion should be added
* `Password` is the Item Password
* `Comment` permits the originator of the Suggestion to give some inputs to the Validator

## Specific case of suggesting a modification of existing Item

If the read-only user wants to suggest a modification, it is mandatory to:

* Use the exact label of the existing Item
* Select the exact folder where the existing Item is stored

Indeed, when a Suggestion is validated, Teampass checks if an existing Item already exist by using those 2 fields.

# Validate a Suggestion

Only a `Manager` or an `Administrator` can validate a Suggestion.

For this use the `plus icon` in front of the Suggestion you want to validate.

* ![Personal folder administration]({{ site.url }}/assets/images/suggestion_system_5.png)

You need to confirm through a specific dialog-box. 

* ![Personal folder administration]({{ site.url }}/assets/images/suggestion_system_6.png)


# Delete a Suggestion

Only a `Manager` or an `Administrator` can delete a Suggestion.

For this use the `minus icon` in front of the Suggestion you want to validate.

* ![Personal folder administration]({{ site.url }}/assets/images/suggestion_system_7.png)

You need to confirm through a specific dialog-box. 

* ![Personal folder administration]({{ site.url }}/assets/images/suggestion_system_8.png)