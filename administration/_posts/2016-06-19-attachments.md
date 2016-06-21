---
layout: post
title: Attachments and Images
category: administration
tags: 
  - upload
  - file
  - attachment
published: true
---

This page describes what are the possible settings for Attachments and Images.

## Principles

In Teampass, it is possible to attach files to each Item.
But an Administrator can setup the scope of allowed attachments.

This can be from `Settings` page, `Uploads` tab.

## File attachments

As many files can be attached to an Item. But each file needs to respect the next settings.

![Attachments]({{ site.baseurl }}/img/posts/attach_1.png)

### File Size

If the file is more than the indicated size, it will be accepted. The size is expressed in Mo.

<span class="fa fa-info"></span>&nbsp;Ensure a consistent value with your server. Don't expect Teampass to allow a 25Mo file size if your server only accepts 2Mo files. 

### File extensions

Teampass requires named extensions, no wildcards `*` is allowed. Extensions are divied in 4 categories:

- Documents
- Images
- Packages
- Others

The separator symbol is the comma `,`.

## Images

Teampass comes with the possibility to store reduced images.

![Attachments]({{ site.baseurl }}/img/posts/attach_2.png)

Once enabled, when an Image will be attached to an Item, it will be reduced using `width`, `height` and `quality` settings as defined.

This permits to ensure consistency in the attached images.
