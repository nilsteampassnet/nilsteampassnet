---
layout:     post
title:      Item attachments
category:   usage
tags:       item attachment file encryption
comments:   true
---

<div class="message">
Files can be attached to an Item.
</div>
<span class="linkmore"></span>

# Introduction

The Item definition includes the possibility to add attachments. Teampass distinguishes 4 categories of attachments: `Documents`, `Images`, `Packages` and `Other`.

> This feature relies on the web browser ability to handle Gear, HTML5, Flash, Silverlight or BrowserPlus. In case, none of those run-times is available then the feature is disabled.

Run-time used is indicated in Home page.

* ![run-time info]({{ site.baseurl }}/assets/images/ia_1.png)

# Administration

This feature cannot be disabled. An Administrator can customize the feature through `Settings` page in `Upload` tab.

## Maximum file size

A maximum file size can be defined if you want to limit the size of attached files. 

<i class="fa fa-bullhorm"></i> Be sure to define a value smaller or equal to the value defined in the server. Please refer to `upload_max_filesize` constant in `php.ini` file.

## File extensions

For each category of attachment, the allowed file extensions can be customized.

* ![run-time info]({{ site.baseurl }}/assets/images/ia_6.png)

## Image resize

In case of the attachment is an image, you can ask Teampass to resize it if its size exceeds the values you have defined.

* ![run-time info]({{ site.baseurl }}/assets/images/ia_7.png)

Resize is performed upon the 3 next criteria:
<ul class="fa-ul">
    <li><i class="fa-li fa fa-check-square"></i>A maximum <b>Width</b> value</li>
    <li><i class="fa-li fa fa-check-square"></i>A maximum <b>Height</b> value</li>
    <li><i class="fa-li fa fa-check-square"></i>A maximum <b>Quality</b> value</li>
</ul>

## Attachment encryption

The files can be encrypted in the server. Refer to [Attachments encryption page]({{ site.baseurl }}/administration/attachments-encryption.html)

# Usage

## How to attach a file to an Item?

Attaching one or several files to an Item is performed through the Item edition/creation dialog-box.

* Open Item dialog-box
* Select `Files & Images` tab
* Click on `Select` button
* Select your files
* Click on `Start uploading files` button
* Check the list of uploaded files
* Close the dialog-box by `Saving`

<i class="fa fa-bullhorm"></i> Saving is mandatory to confirm the upload of the files.

* ![Uploading files]({{ site.baseurl }}/assets/images/ia_2.png)

## How to delete an attachment?

* Open Item dialog-box
* Select `Files & Images` tab
* In the attachments list, click the `delete` icon in front of the file to delete
* Close the dialog-box by `Saving`

<i class="fa fa-bullhorm"></i> Saving is mandatory to confirm the deletion.

* ![Deleting a file]({{ site.baseurl }}/assets/images/ia_3.png)
* ![Deleting a file]({{ site.baseurl }}/assets/images/ia_5.png)

## How to download an attachment?

When browsing an Item, you can click on one of the attachment to start the download of the file.

* ![Downloading]({{ site.baseurl }}/assets/images/ia_4.png)