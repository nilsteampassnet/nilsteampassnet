---
layout: page
title: Options explained
subtitle: List and explanation of main Teampass options
published: true
comments: true
---
<a name="top"></a>

This page lists all major options that can be selected through the `Settings` page.

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
- [Folders with identical name](#folder-same-name)
- [Items with identical label](#item-same-name)
- [Identical items in Folder](#similar-items-one-folder)
- [Simplify Tree](#simple-tree)
- [New folder rights inheritance](#folder-rights)
- [Adding more fields to Items using Categories](#categories))
- [Manage sub-folders of allowed parent-folder](#manage-sub-folders)
- [Passwords can expire after a date or a number of displays](#pwd-expiration)
- [Automatically delete items](#item-auto-deletion)
- [Printing out in PDF file](#pdf-file)
- [Importing CSV files](#importing-csv)
- [Importing Keepass files](#importing-keepass)
- [Allow Item modification](#every-one-can-modify)
- [Restricted access to Item](#restricted-access)
- [Fast copy icons](#fast-copy)
- [Number of Items loaded in one query](#items-number-loaded)
- [Manual insertions in History log](#history-manual-insertion)
- [Off-line mode](#Offline-mode)
- [Changing user password on remote Linux server](#remote-linux-pwd-change)

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

When opening the `Information` page when logged as an Administrator, some information such as `last Teampass version` are loaded from the Teampass server.

By default this is enabled but you can disable it.
This will not permit you to be warned when a new release is available. 

[Back to Top](#top)

----------

### <a name="failed-edition"></a>Failed item edition

Teampass is a multi-users tool. That means that several users may access an item at the same time. In order to prevent against item edition by several users in parallel, Teampass allocates a token to the 1st user that started the edition. 
This will reject an edition of another user.
When the current editor closes or save the item, the token is deleted.

This option permits to define a duration in **minutes** during which no other edition will be allowed, but when delay is reached, the token will be deleted and current user will not be able to save anymore.
In other words, this permits to ensure that the editor hasn’t forgotten to close the edition.

By default, the value is set to `0`. This disables this feature and only an Administrator can remove the token.
A good value could be 10 minutes as we can assume that no one will modify an item in more than 10 minutes.

[Back to Top](#top)

----------

### <a name="otv-expiration"></a>One Time View link expiration

One Time View permits a User to share an Item with a person that doesn't have access to Teampass. This person receives an email that contains a link. This link permits to open a specific page in Teampass that contains the Item information.

This link can only be open once as it is deleted once displayed. This option permits to define the number of **days** the link is valid. In other words, once the delay is passed, the link is removed and the person will reached an empty page.

[Back to Top](#top)

----------

### <a name="managers-edit-delete"></a>Managers can edit and delete items

Managers are normal Users with some more rights on Folders, Groups and Users configuration.
By enabling this option, they will also be allowed to `edit` and `delete` any Items they are allowed to access.

By default, this option is **enabled**. 

[Back to Top](#top)

----------

### <a name="folder-same-name"></a>Folders with identical name

By default, it is not allowed to have 2 Folders with the same name. Nevertheless this restriction can be by-passed by enabling it.

As a result, no control will be performed on Folder names while creating or editing them. And 2 or more folders may have the same name inside Teampass tree structure.

[Back to Top](#top)

----------

### <a name="item-same-name"></a>Items with identical label

By default, it is not allowed to have 2 Items with the same label. Nevertheless this restriction can be by-passed by enabling it.
No control will be performed on Item labels while creating or editing them as long as they are located in different Folders.

As a result, several Items may have the same label while they are located in different Folders. But no duplicate one will be allowed in one Folder.

[Back to Top](#top)

----------

### <a name="similar-items-one-folder"></a>Identical items in Folder

As seen in previous point, similar Items in one Folder is not possible by default in Teampass. By enabling this feature, users may create Items with similar label inside a unique Folder.

[Back to Top](#top)

----------

### <a name="simple-tree"></a>Simplify Tree

The folders Tree is shown as a complete structure. As a consequence, a User (depending on his access rights) may see Folders that he will not be able to access. By clicking on it, a warning message indicating the User that he is not allowed to access the folder will be displayed.

In case of simple Tree structure, it could be useful to enable this option, so that Users only see the Folders they are allowed to access.

But this might generate inconsistencies for the Users in complex Tree structure. Indeed if a User has access to a sub-folder of a folder (to which he is not allowed to access), the Tree structure will not show the top-folder which will give a wrong view of the path to User.
But this is only a view, there is no incidence on the data and contain.

[Back to Top](#top)

----------

### <a name="folder-rights"></a>New folder rights inheritance

When creating a new Folder, all existing User-Groups who have access to parent-folder will also receive the access rights to this new sub-folder.

*As an example, if parent-folder can be accessed by User-Groups U1 and U3, then those 2 User-Groups will have access to this new sub-folder (respecting the type of access defined).*

By enabling this option, all User-Groups the creator belongs to will also receive the `Write` access on this new sub-folder.

*As an example, if Creator belongs to User-Groups U1, U2 and U4, then all users belonging to those 3 User-Groups will also have Write access on this new sub-folder.*

[Back to Top](#top)

----------

### <a name="categories"></a>Adding more fields to Items using Categories

It is possible to define custom fields to be added to Items definition. As example, `URL` field is by designed existing in Teampass but for a specific type of Items, it could be requested to have a `Credit Card PIN` field. In this case, it could be interesting to enable this option.

By using the tab `Categories`, it is possible to define Categories of new fields. Each Category is then related to Folders.
By this it is possible to request specific types of fields to be added to the Item Definition.

Notice that **all custom fields inputs are encrypted** in the database.

By default, this option is **disabled**. 

[Read more about the Categories usage](2013-03-25-custom-categories-and-fields)

[Back to Top](#top)

----------

### <a name="manage-sub-folders"></a>Manage sub-folders of allowed parent-folder

Users cannot `edit` and/or `delete` Folders they have not created.

Nevertheless this can be by-passed when this option is enabled.
So if enabled, Users having access to a top-folder will be allowed to `edit` and/or `delete` any sub-folders.

By default, this option is **disabled**. 

[Back to Top](#top)

----------

### <a name="pwd-expiration"></a>Passwords can expire after a period of time

Teampass permits to define a renewal period by Folder.
Meaning that if option is enabled and a period of renewal  set (in days), password defined in an Item will require to be updated at least once the renewal period is passed.

If not updated, the Item will remain hidden for Users. Only the Creator and Managers will see it. 

By default, this option is **disabled**. 

[Back to Top](#top)

----------

### <a name="item-auto-deletion"></a>Automatically delete Items

Once created, an Item can be displayed without any limit of time.

Nevertheless, Teampass permits to define a pre-defined limit of time after which the Item will be deleted (pushed to the Recycle Bin). This limit of time can be defined as being a `date` or a `maximum counter of visualization`.

This date of counter is defined in the Item definition dialogbox.

By default, this option is **disabled**. 

[Back to Top](#top)

----------

### <a name="pdf-file"></a>Printing out in PDF file

For any reason, Teampass permits to export a list of Items in a PDF file. For security reasons, a password is asked to protect the PDF file and this action is logged inside the database.
Exporting to a PDF file starts with selecting the folders from which the Items list will be exported.

Exporting to PDF can be limited to specific User-Group.

By default, this option is **disabled**. 

[Back to Top](#top)

----------

### <a name="importing-csv"></a>Importing CSV files

Teampass permits to import Items through **CSV** file. 
Currently the format is fixed and needs to be respected to perform a successful importation. 

The CSV file is defined as bellow:

- it must contain a header
- it must be made of 5 columns:
    - Label
    - Login
    - Password
    - URL
    - Comments
- the separator to use is the comma symbol ` , `
- the column enclosure symbol is the double-quotes `"`

The importation is performed in 2 steps:

- Step 1 - the CSV file is read and existing Items displayed,
- Step 2 - the user selects the Items to be imported.

Notice that importation of Items with CSV file will create the new Items inside the selected Folder.

By default, this option is **disabled**. 

[Back to Top](#top)

----------

### <a name="importing-keepass"></a>Importing Keepass files

Teampass permits to import Items through **Keepass XML** file.  
This file is generated out of Keepass using `Export` feature and by selected `Keepass XML` format.

Once selected the destination Folder and the file to use, the importation is performed automatically. This means that all Folders and Items existing in the XML file will be created inside the destination Folder.

<span class="fa fa-info"></span>&nbsp;Notice that if Keepass folder structure is composed of several sub-folders with the same name in the same folder, then all Items will be created in one unique sub-folder.

By default, this option is **disabled**. 

[Back to Top](#top)

----------

### <a name="every-one-can-modify"></a>Allow Item modification

In some cases, it could be useful to give `Edition` right on a specific Item without performing changes on `User-Groups / Folders` configuration.

This option permits the Item Owner to open its edition to **Every One** or define a **restricted list of possible editor**s. The defined list can be composed of one or several Users, and/or one or several User-Groups.

By default, this option is **disabled**. 

[Back to Top](#top)

----------

### <a name="restricted-access"></a>Restrict access to Item

In some cases, it could be useful to restrict access of an Item without performing changes on `User-Groups / Folders` configuration.

This option permits the Owner of an Item to define **who can access the Item**. The defined list can be composed of one or several Users, and/or one or several User-Groups.

By default, this option is **disabled**. 

[Back to Top](#top)

----------

### <a name="fast-copy"></a>Fast copy icons

While displaying the list of Items inside a Folder, it is possible to associate small icons permitting to:

- password copy in clipboard, 
- login copy in clipboard,
- add Item in Favorites list

This option requires more resources on server (perform test before enabling).

By default, this option is **disabled**. 

[Back to Top](#top)

----------

### <a name="items-number-loaded"></a>Number of Items loaded in one query

The Items belonging to a Folder are loaded sequentially in order to prevent a freeze while clicking on a Folder in case of huge number of Items.

This option permits to define the number of Items Teampass will load in one query. By default, an optimized number is calculated, but you may decide your own one.

<span class="fa fa-info"></span>&nbsp;In a general manner, it is recommended to keep a reasonable number of Items in on Folder in order to prevent against painful loading time. Teampass has no limit in term of Folders so organize your structure in a smart way.


[Back to Top](#top)

----------

### <a name="history-manual-insertion"></a>Manual insertions in History log

Teampass logs all actions performed on Items. 

In some cases, it could be needed to add specific information inside the log (for example for imported Items).

This option permits a User to add an input inside the History log of an Item.

By default, this option is **disabled**. 

[Back to Top](#top)

----------

### <a name="offline-mode"></a>Off-line mode

Off-line mode option permits to export inside an html file that can be consulted without being connected to Teampass using a web-browser.

If enabled, a User can export a list of folders into this html file. A password will be requested in order to encrypt once more the passwords inside the html file. This password will also be requested to decrypt the password in the html file.

Advantage of this file is that the User can access the passwords even if not connected to the Teampass server, and even without internet on his computer.

<span class="fa fa-info"></span>&nbsp;The Administrator can define the minimum complexity level the password needs to fulfil.

By default, this option is **disabled**. 

[Back to Top](#top)

----------

### <a name="remote-linux-pwd-change"></a>Changing user password on remote Linux server

This option permits to change the password of a User account in a remote Linux server.

It has been developed to ensure password synchronization between server user account and Teampass. Meaning that if the Item concerns an Account on a remote Linux server, while changing the the password under Teampass, it can be automatically changed on the server.

Teampass can either do this as:

- **one-shot** - the user decides to update the server account and Teampass performs the change
- **automatic** - based upon a task and a frequency, Teampass automatically changes the password in Teampass and on the server.

<span class="fa fa-info"></span>&nbsp;This requires an SSH connection.

By default, this option is **disabled**. 

[Back to Top](#top)
