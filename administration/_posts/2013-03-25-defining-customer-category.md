---
layout: post
title: Defining Categories and Fields
category: administration
tags: 
  - fields
  - folders
  - categories
  - gui
comments: true
noToc: false
published: true
---

This page describes how to manage custom Categories for Items.

Read page [custom Categories and Fields](/administration/2013-03-25-custom-categories-and-fields.html) for definition.

## Administration

`Categories for Items` is an option and needs to be enabled.
For this, open `Settings` page and select tab `Customize`.
Option is called `Authorize Items to be completed with more Fields (by Categories)`.

Notice that you can create Categories and Fields even if the option is not enabled. The option only impacts the display or not of those categories while using Items.

## GUI

The GUI is made of 2 zones. 

The first one shows a Tree made of the Categories and the related Fields.

The second one is dedicated for Categories management (with specific actions).

![Categories]({{ site.baseurl }}/img/posts/cat_1.png)

### Managing Categories

The Categories are managed through the bottom box.

![Categories]({{ site.baseurl }}/img/posts/cat_2.png)

#### Adding new Category

Enter the label of Category and click `Add Category` button.
This new Category will be added in the Tree in alphabetic order.

#### Renaming and Deleting

Those 2 actions are performed the same way. Do:

* select the Category (its name should be added in the text box),
* modify the label (in case of a renaming action),
* click the button corresponding to your action

<span class="fa fa-warning"></span>&nbsp;Notice that when deleting a Category, all attached Fields are deleted, as all the values in the Database related the Items.

#### Moving

You can decide to move the Fields from one Category to another. Do:

* select the Category (its name should be added in the text box),
* select the Category target (with the drop list),
* click the button.

#### Organizing the Categories

You can decide to organize the Categories in a custom order. For this, use the small text box in front of the label and enter a number.
The Categories will be sorted by number as primary criteria and by alphabetic as second criteria.

![Categories]({{ site.baseurl }}/img/posts/cat_3.png) 

#### Associating a Folder to a Category

You need to relate a Category to Folders. for this,

* use the Tree
* click the icon "Associated folders"
* select the Folders you want (multiple selection is possible)
* click OK button to confirm

The Folders are now associated to the select Category.

![Categories]({{ site.baseurl }}/img/posts/cat_4.png) 

### Managing Fields

The Fields are managed through the bottom box.

The exact same feature described above are valid for Fields. The unique difference concerns the Field creation.

#### Adding new Field

Adding a new field in a Category is performed as this:

* use the Tree,
* spot the Category you want to improve,
* click the icon +,
* enter the label of the field,
* confirm with the button
