Open Source Social Network
======================================
[![Open Source Love](https://badges.frapsoft.com/os/v2/open-source.svg?v=102)](https://www.opensource-socialnetwork.org/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://www.opensource-socialnetwork.org/)
[![Build Status](https://travis-ci.org/opensource-socialnetwork/opensource-socialnetwork.svg?branch=v5.x)](https://travis-ci.org/opensource-socialnetwork/opensource-socialnetwork)
[![Download Latest](https://img.shields.io/badge/Download-Latest%20Version-blue.svg)](https://www.opensource-socialnetwork.org/download)
[![DeepScan grade](https://deepscan.io/api/teams/4774/projects/6525/branches/54923/badge/grade.svg)](https://deepscan.io/dashboard#view=project&tid=4774&pid=6525&bid=54923)

Opensource-Socialnetwork (OSSN) is a social networking software written in PHP. It allows you to make a social networking website and helps your members build social relationships, with people who share similar professional or personal interests. It is available in 16 international languages.

Front-End Features
===================
* User Registration
* User Login
* Profile 
* Profile Photo
* Profile Cover
* Add/Remove Friends
* Live Chat
* Wall posts
* Photos
* Ads
* Groups
* Tag friends in posts
* User block system
* User poke system
* Comments
* Likes
* Reactions
* Photos in comments.
* Group cover photos
* Repostion Profile/Group cover
* Notifications
* Friend Requests
* Chat Bar
* Invite Friends
* Embed Videos
* Smilies
* SitePages (terms, privacy, about)
* Site Search
* Reset Password
* Newsfeed page
* Post Edit
* Comment Edit
* Mobile Friendly
* A photo gallery view.
* Emojii Support

Backend Features
=================

* Admin Dashboard for site overview
* Online users count (male/female) graph
* Total site users count (by months) graph
* Update Notification
* Add User
* Remove User
* Edit User
* Ads Manager
* Site Cache Settings
* Site Basic Settings
* Unvalidated users
* Manually validate unvalidated users
* and much more components settings

Installation
============

## Install LAMP
> LAMP (Linux, Apache, MySQL, PHP) >
1. Install Apache
```
sudo apt install apache2
sudo service apache2 restart
```
2. Install MySQL
```
sudo apt -y install mysql-server mysql-client
sudo mysql -u root
sudo mysql_secure_installation
```
3. Install PHP
```
sudo apt -y install php7.2
sudo apt -y install libapache2-mod-php7.2
sudo apt -y install php7.2-mysql
sudo apt install php-pear php7.2-curl php7.2-dev php7.2-gd php7.2-mbstring php7.2-zip php7.2-mysql php7.2-xml
```
## Create database
```
sudo mysql -u root -p
create user 'ossn'@'localhost' identified by 'password';
create database ossn;
mysql> GRANT ALL PRIVILEGES ON ossn.* TO 'ossn'@'localhost' IDENTIFIED BY 'password' WITH GRANT OPTION;
```
## Source code
```
sudo apt install -y git
git clone https://github.com/Greenhat1998/opensource-socialnetwork
```
Copy all file into /var/www/html (with root permission) and create ossn_data folder
```
mkdir /var/www/ossn_data
chgrp www-data /var/www/html
chgrp www-data /var/www/ossn_data
chmod g+w /var/www/html
chmod g+w /var/www/ossn_data
a2enmod rewrite
service apache2 restart
```
## Config
Access http://localhost/installation to config you website

DEMO
====
http://demo.opensource-socialnetwork.org/
