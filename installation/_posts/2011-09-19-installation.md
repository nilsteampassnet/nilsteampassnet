---
layout: 		post
title: 			Teampass installation
category: 	installation
tags:				installation
---

<p class="message">
    This page describes how to install TeamPass whatever the type of server you are using.
</p>
<span class="linkmore"></span>

# Preparation

* Download lastest package,
* Unzip package into a temporary folder,
* Upload package on your server,
* Enter url `http://your_domain/teampass/install/install.php`

# Step 1

It's an introduction page with some recommendations and the licence display.

# Step 2

Check that the given database credentials are correct and permit Teampass to get connected to the database.

It is required to give the next credentials:

- **Server name** (ex: localhost)
- **Database name** (it is recommended to have a dedicated database for Teampass. Ex: teampass)
- **User** (it is recommended that this user has ROOT privileges on Teampass database) 
- **Password**
- **Tables prefix**

# Step 3

Defining various points for Teampass definition.

Among other, the most important are:

* **Saltkey** is the key that will be used to encrypt and decrypt all encrypted objects in database. This key needs to be complex to ensure a good security of the encryption. It is highly recommended to use the `Generator`.
* **SK path** is the path in your server where the file containing the Saltkey will be stored. It can be any path of your server. It is recommended that this path is outside the `WWW domain` of your server for security reasons.
* **Email settings** can be defined in this page but you may define them after through specific administration page.

# Step 4

This step permits the tables creation and data copy.

# Step 5

This step permits to create the SK.php file and to copy it at the specific indicated path.

Notice that if you are facing an error at this step, please be sure that this path is accessible for the user and that the expected rights are also defined (777).

# Done

Once the previous steps are done, Teampass is now installed on your server.

The by-default login credentials are `admin`.

