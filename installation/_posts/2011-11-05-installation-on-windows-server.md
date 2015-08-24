---
layout: page
title: Installing TeamPass on Windows server
category:		installation
tags:				installation windows
---

<p class="message">
    This page describes how to install TeamPass on a Windows server.
</p>
<span class="linkmore"></span>

In order to install TeamPass on a Windows server, you need to first have an Apache server with MySql and PHP. 
You can either install each of those components one by one, or directly use a full 'All in One' package such as Xampp, WampServer, etc.
> This guide is based upon WampServer, but is rather the same with any other package.

# Install your Apache server

* Download the last version of WampServer
* Launch installation (you can follow installation directly from the Help page of the editor)
* Once installed, start your server and you should see the wampserver icon in green. As shown in next screen capture.

# Prepare TeamPass environment

## Activate PHP mcrypt extension

* Do a click on the WampServer icon
* In the dialogbox, select PHP >PHP extensions and click on  `php_mcrypt`

## Set MySQL database Administrator

* Open PhpMyAdmin (click on the WampServer icon and select PhpMyAdmin)
* In the 'Create new database' section, enter your database name (for example `teampass`) and select `UTF8_general_ci` as collation.
* Click on `Create` button

##Set MySQL database Administrator

We'll now create a specific Administrator to this database

* Click on 'localhost' in order to get back to home page
* Select 'Privileges' tab
* Click on 'Add a new user' link
* Enter the login information (I suggest to create a user `teampass_admin` for better understanding of what is this user)
* Do not give any rights/privileges at this level of the user creation
* Click on 'Go' button

Now it's time to set some privileges to this user.

* From Home page, click on `Privileges` tab
* Click on 'Edit privileges' button corresponding to the `teampass_admin` user
* Click on 'Check All' link
wampserver_green
Create database
Edit privileges of user
Set privileges to user

* Validate by clicking on button `Go`

## Upload files

* Download TeamPass package
* Unzip it in a temporary folder
* If your installation is a local one, copy the folder TeamPass in folder `<wampserver_installation_path>/www`. If it is a remote server, use your FTP software to upload the TeamPass folder in `html_public` folder

## Ready to install TeamPass

* With your favorite web browser, get to `http://<your_teampass_url>`
* Follow instruction given by the installation script

