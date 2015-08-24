---
layout: 		post
title: 			Change Administrator usage
category: 		administration usage
tags:			administration user
toc:			false
---

<p class="message">
    The Administrator user type can also manage Items.
</p>
<span class="linkmore"></span>

> An Administrator has by default no access to Items.

If for any reason, you want an Administrator to have access to Items and becoming a "normal user", then you need to do the next change.

* Open file `include.php` in folder `/includes`
* Change sentence `$k['admin_full_right'] = true;` to `$k['admin_full_right'] = false;`

Nevertheless, it is not a recommended way to do because the Administrator is in this case able to access any Items because he/she has access to all Rights configuration.
So it should reserved to special cases of Teampass usage.