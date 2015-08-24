---
layout:     post
title:      Attachments encryption
category:   administration
tags:       attachment encryption item
comments:   true
noToc:      false
---

<div class="message">
Teampass permits you to encrypt the Item attachments.
</div>
<span class="linkmore"></span>

# Introduction

By default, the files attached to Items are not encrypted. For security purpose, it could be good to encrypt those files on the server.
For this, the feature `Enable encryption of Items attachments` needs to be enabled in the Settings page. 

> Read carefully next chapter in case you change this option when attachments already exist.

The encryption is performed using Teampass Saltkey. Be careful, this requires more server resources.

# Changing encryption strategy in production mode

If you decide to change strategy while attachments already exist, it is then mandatory to apply the strategy on those files.
This has to be done in both cases.

If previous status was `Disabled`, then you need to encrypt all existing files.
If previous status was `Enabled`, then you need to decrypt all existing files.

# How to apply new strategy?

Before starting this, we recommend to:

* set Teampass under Maintenance so that no user are connected
* make a copy of the folder `Upload`

Follow next steps:

1. Open Settings page
2. Select tab Misc Operations
3. Spot action `Encrypt or Decrypt the Items attachments`
4. Click on the button corresponding to your new strategy