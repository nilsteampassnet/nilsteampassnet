---
layout: post
title: API access through third party application
category: feature
tags: feature api
published: true
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

`<url to teampass>/api/index.php/read/category/<folder id1>;<folder id2>;<folder id3>?apikey=<valid api key>`

The separator symbol is the comma ` ; `.

The answer would be exactly the same as in the previous example.

## Read specific Items

To get the information about one specific Item, use URL

`<url to teampass>/api/index.php/read/items/<item id1>;<item id2>;<item id3>?apikey=<valid api key>`

The separator symbol is the comma ` ; `.

The answer would be exactly the same as in the previous example.

# Add new Item

It is possible to add a new Item using the API. Use URL

`<url to teampass>/api/index.php/add/item/<label>;<password>;<description>;<folder id>;<login>;<email>;<url>;<tags>;<any one can modify>?apikey=<valid api key>`

The separator symbol is the comma ` ; `.

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


# Add new User
 
The API permits to add a new user in Teampass.

## Call format
The URL to send has to be preformated as shown bellow.
 
`<url to teampass>/api/index.php/add/user/<LOGIN>;<NAME>;<LASTNAME>;<PASSWORD>;<EMAIL>;<ADMINISTRATED_BY>;<READ_ONLY>;<ROLE1|ROLE2|...>;<IS_ADMIN>;<ISMANAGER>;<PERSONAL_FOLDER>?apikey=<VALID API KEY>`
 
The separator symbol is the comma ` ; `.
 
*Some limitations*:
 
* for `READ_ONLY`, `IS_ADMIN`, `IS_MANAGER`, `PERSONAL_FOLDER`, accepted value is `1` for TRUE and `0` for FALSE
* for `ADMINISTRATED_BY` and `ROLE1`, accepted value is the real label (not the IDs)

## Example

The next URL ...

```
https://127.0.0.1/teampass/api/index.php/add/user/U4;Nils;Laumaille;test;nils@teampass.net;U1;0;Managers|Users;0;1;1?apikey=sae6iekahxiseL3viShoo0chahc1ievei8aequi
```

... creates a user with next characteristics:
* `Login`: U4
* `Name`: Nils
* `Lastname`: Laumaille
* `Password`: test
* `Email`: nils@teampass.net
* `Is administrated by`: U1
* `Is read-only`: No
* `Roles`: Managers|User
* `Is administrator`: No
* `Is manager`: Yes
* `Has personal folder`: Yes

# Delete Item

**Warning** The API will delete the data from database.

## Deleting all items inside folders

This chapter explains how to delete all Items inside one or several folders.

### Call format

`<url to teampass>/api/index.php/delete/folder/<folder_id1;folder_id2;folder_id3>?apikey=<VALID API KEY>`

Use the keywords `delete/folder/`

Followed by the IDs of the folders in which the Items will be deleted.
You can indicate several folders if you separate the folder IDs by a comma ` ; `.

### Example 

```
https://127.0.0.1/teampass/api/index.php/delete/folder/3;48;62?apikey=sae6iekahxiseL3viShoo0chahc1ievei8aequi
```

This URL will delete Items inside folders with IDs 3, 48 and 62.

## Deleting specific items

This chapter explains how to delete specific Items.

### Call format

`<url to teampass>/api/index.php/delete/item/<item_id1;item_id2;item_id3>?apikey=<VALID API KEY>`

Use the keywords `delete/item/`

Followed by the IDs of the items to be deleted.
You can indicate several items if you separate the item IDs by a comma ` ; `.

### Example 

```
https://127.0.0.1/teampass/api/index.php/delete/item/3;12;16?apikey=sae6iekahxiseL3viShoo0chahc1ievei8aequi
```

This URL will delete Items with IDs 3, 12 and 16.