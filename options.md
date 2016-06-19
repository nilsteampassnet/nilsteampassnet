---
layout: page
title: Options explained
subtitle: List and explanation of main Teampass options
published: true
comments: true
---
<a name="top"></a>

This page lists all major options that can be selected through the `Settings` and `Customize` pages.

- [Maintenance Mode](#maintenance)
- [Session expiration](#session)
- [Encrypted Client-Server exchanges](#encrypt-exchanges)
- [Attachments encryption](#attach-encryption)
- [Knowledge Base ](#kb)
- [Item Suggestion](#suggestion)
- [information about Teampass](#info)
- [Failed item edition](#failed-edition)
- [One Time View link expiration](#otv-expiration)
- [Managers can edit and delete items](#managers-edit-delete)

----------

### <a name="maintenance"></a>Maintenance Mode

When enabled all users except Administrators will be logged out of Teampass.
It is not possible to get logged in anymore.

This mode could be useful when:

- upgrading Teampass
- defining or changing the structure of folders
- performing other specific actions

[Back to Top](#top)

----------

### <a name="session"></a>Session expiration

A user session period corresponds to the period of time the user is logged in Teampass before being automatically logged out. Once time session is over, the active session of the user is closed.
The remaining time (count down) is visible in the footer.

One minute before expiration, a warning message is displayed to the user asking him to renew the session period.
A user can also increment the session at any moment using `Extend session by 1 hour` in the top menu bar.

This field requires a numerical value in **minutes**. Its default value is 60 minutes (1 hour).


[Back to Top](#top)

----------

### <a name="encrypt-exchanges"></a>Encrypted Client-Server exchanges

Encrypted client-server exchanges option permits to encrypt exchanges between the Client and the Server.
This concerns exchanges (posts and answers) that contain important data such as names, ids, passwords, ...

If your Teampass is not in a safe Network, it is highly recommended to have this option enabled.

By default, the option is enabled.

[Back to Top](#top)

----------

### <a name="attach-encryption"></a>Attachments encryption



[Back to Top](#top)

----------

### <a name="kb"></a>Knowledge Base 

Knowledge Base is a space where users can create kind of tickets which can contain any kind of information that can be related to existing Items.
The idea behind it is to have a verbose space that comes with the Items.

[Back to Top](#top)

----------

### <a name="suggestion"></a>Item Suggestion

Suggestion is a system permitting any User (and especially the Read-Only ones) to suggest new Items to be added in the list of Items. 
Once created, a Manager can approve or reject the suggestion.

[Read More about Suggestion system](2014-05-24-suggestion-system)

[Back to Top](#top)

----------

### <a name="info"></a>information about Teampass

When opening the `Information` page when logged as an Administrator, some informations such as `last Teampass version` are loaded from the Teampass server.

By default this is enabled but you can disable it.
This will not permit you to be warned when a new release is available. 

[Back to Top](#top)

----------

### <a name="failed-edition"></a>Failed item edition

Teampass is a multi-users tool. That means that several users may access an item at the same time. In order to prevent against item edition by several users in parallel, Teampass allocates a token to the 1st user that started the edition. 
This will reject an edition of another user.
When the current editor close or save the item, the token is deleted.

This option permits to define a duration in **minutes** during which no other edition will be allowed, but when delay is reached, the token will be deleted and current user will not be able to save anymore.
In other words, this permits to ensure that the editor haven't forgotten to close the edition.

By default, the value is set to `0`. This disable this feature and only an Administrator can remove the token.
A good value could be 10 minutes as we can assume that no one will modify an item in more than 10 minutes.

[Back to Top](#top)

----------

### <a name="otv-expiration"></a>One Time View link expiration

One Time View permits a User to share an Item with a person that doesn't have access to Teampass. This person receives an email that contains a link. This link permits to open a specific page in Teampass that contains the Item informations.

This link can only be open once as it is deleted once displayed. This option permits to define the number of **days** the link is valid. In other words, once the delay is passed, the link is removed and the person will reached an empty page.

[Back to Top](#top)

----------

### <a name="managers-edit-delete"></a>Managers can edit and delete items

By default, Managers are normal Users plus some rights concerning Folders, Groups and Users configuration.
By enabling this option, they will also be allowed to `edit` and `delete` any Items they are allowed to access.

By default, this option is **enabled**. 

[Back to Top](#top)