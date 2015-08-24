---
layout: 		post
title: 			API access through third party application
category:		feature
tags:			feature api
---

<p class="message">
    This page describes how to use API access.
</p>
<span class="linkmore"></span>

# Goal?

The goal of the API is to permit an access to Teampass Items from a third party application.

At this level of development, the API is able to handle READ and DELETE Items.

The call is performed with a `GET` query and the send back data is at `json` format.

# Read data

## Read one Category

Reading the content of a Category is performed by accessing the URL

`<url to teampass>/api/index.php/read/category/<folder id>?apikey=<valid api key>`

The answer would be

`{
	"1":{
		"label":"I1",
		"login":"",
		"pw":"&XZcww1`"
	},
	"2":{
		"label":"Google",
		"login":"Me",
		"pw":"nid6YA$B"
	}
}`

## Read several Category

Reading the content of several Category is performed by accessing the URL

`<url to teampass>/api/index.php/read/category/<folder id1>,<folder id2>,<folder id3>?apikey=<valid api key>`

The separator symbol is the comma ` , `.

The answer would be exactly the same as in the previous example.

## Read specific Items

To get the information about one specific Item, use URL

`<url to teampass>/api/index.php/read/items/<item id1>,<item id2>,<item id3>?apikey=<valid api key>`

The separator symbol is the comma ` , `.

The answer would be exactly the same as in the previous example.

# Add new Item

It is possible to add a new Item using the API. Use URL

`<url to teampass>/api/index.php/add/item/<label>,<password>,<description>,<folder id>,<login>,<email>,<url>,<tags>,<any one can modify>?apikey=<valid api key>`

The separator symbol is the comma ` , `.

*Some limitations*:

* `URL` should NOT include `http://`. Indeed this would break the initial url.
* `tags` field can be used for multiple tags and they need to be separated by a space.
* `any one can modify` is a boolean and accepts value `1` for `TRUE` and value `0` for `FALSE`.

Notice that if a similar Label exists, the add request will fail.

# Authentication credentials for a web page

The API returns the `LOGIN` and `PASSWORD` based upon an `URL` sent in entry.

## Call format

`<url to teampass>/api/index.php/auth/<PROTOCOL>/<URL>/<user login>/<user password>?apikey=<VALID API KEY>`

With:

* < PROTOCOL > : is the protocol used for the URL (example: http|https|ftp|...)
* < URL > : is the URL without the protocol (example: http://www.teampass.net becomes www.teampass.net)
* < user login > : user's login
* < user password > : user clear password
* < VALID API KEY > : api key for access validation

```
Example: https://127.0.0.1/teampass/api/index.php/auth/http/www.zadig-tge.adp.com/U1/test?apikey=chahthait5Aidood6johh6Avufieb6ohpaixain
```
 
## Returned answer
 
The format sent back is JSON.
If several entries exist for one URL then all possibilities will be sent back.
 
Example: {"<item_id>":{"label":"<pass#1>","login":"<login#1>","pw":"<pwd#1>"},"<item_id>":{"label":"<pass#2>","login":"<login#2>","pw":"<pwd#2>"}}