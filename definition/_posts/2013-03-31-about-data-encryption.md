---
layout:     post
title:      About data encryption
category:   definition
tags:       encryption categories
comments:   true
---

<div class="message">
Teampass secures your data by encrypting them following rules defined in this page.
</div>
<span class="linkmore"></span>

# Encryption scope

Encryption is not performed on each database Tables fields. This is for performance reason.
Next fields are encrypted in the database:

* `Password` value
* `Custom fields` value

All other fields are in clear text in the database.

# Encryption protocol

The encryption algorithm used in AES-256 cipher IV based upon the `SALTKEY` defined during the installation of Teampass. This ensures a very good level of security of the encrypted strings against brute force.
You may read more on [AES-256 cipher](http://fr.wikipedia.org/wiki/Advanced_Encryption_Standard).