---
layout:			post
title:  		How to communicate an Error log?
category:		usage
tags:			usage bug
---

<div style="message">
When you open an issue in Github, it could be good that you join the error generated on your server. If you don't know how to perform that, here is some tips you could follow.
</div>
<span class="linkmore"></span>

# Use Firebug
<strong>Firebug</strong> is an extension for at least web browsers Chrome and Firefox. You can securely use it and only activate it when you want to report issues you have discovered using Teampass.

Get <b>[Firebug][getfirebug]</b>!

Once installed, you will get a small `bug` in the menu bar of the browser.
![Firebug enabled]({{ site.url }}/assets/images/2014-02-09-02.png)


# Activate options

At the very begining, you should check that next options are activated in Firebug.

* Console should be activated
* Script should be activated
	
# How to get the error message

When you are facing an issue using Teampass, you should:

* Enable Firebug
* It should normally open the `Firebug dialogbox` (by default in the low part of your browser)
* Relaunch the action that causes the issue
* Open tab `Console`
* Identify the POST that has failed (it should in RED)
* Expand using the symbol ` + `
* Select tab `Response`
* Make `Copy response body` using right-click mouse
* Paste this in the github message
* Make `Copy location with parameters` using right-click mouse
* Paste this in the github message


Don't forget to disable Firebug after this ;-)

[getfirebug]: http://getfirebug.com/
