How to get started
==============
Getting the code
-------------------
1.	Download Git and make sure your account has working SSH keys
2. 	From the command line, set your current working directory to be the 
	directory above where you want the project to be. For example, if you 
	are going to run this as a subfolder on your local development
	server, select the webserver's root. For example:
	
	`cd /Applications/XAMPP/xamppfiles/htdocs/`
3. 	Download a clone of the repository, replacing USERNAME with your
	GitHub username.
	
	`git clone https://USERNAME@github.com/giftflow/giftflow.git`
	
	This will create a folder in your working directory called giftflow and
	download the latest version of the repository to it.
4.	Now change your working directory to be the folder you just cloned:
	
	`cd giftflow`
	
Configuration
----------------
1.	*Create the database*
	
	Create a database called gift and import the SQL found in the repository.
	`/giftflow/gift.sql` contains the structure of the database and `/giftflow/data.sql` contains some
	sample data.

2.	*Edit config.php* 
	
	This file is located at `/giftflow/system/application/config/config.php`
	
	You may need to edit the first two entries in the config array, located at lines 14 and 15: 
	`$config['base_url']` and `$config['base_path']`. Change their values to reflect 
	your installation.

3.	*Edit database.php*
	
	This file is located at `/giftflow/system/application/config/database.php`
	
	Here you should edit the database connection information to suit your needs. By default, it
	looks to localhost for a database named gift using the username root with a blank password.

Using Git
=======

[GitHub has a good introduction to using Git here](http://learn.github.com/). Below some of the most
basic tasks will be covered.

Fetching the latest version of the repository
--------------------------------------------------
`git pull origin master`

Pushing your changes to the master branch
--------------------------------------------------
`git push origin master`