# Project5-Linux-Server-Configuration

#Overview

This project takes a baseline installation of a Linux distribution on a virtual machine and prepares it to host a web application by installing updates, securing it from a number of attack vectors, and installing/configuring web and database servers.

##HTTP

The web application, The Sports Catalog, is hosted via HTTP at the server's IP address: 52.33.235.211.

http://52.33.235.211/


##SSH

To access the server, SSH into the server by executing the command:

ssh -p 2200 -i [RSA_FILE] grader@52.33.235.211

Ensure the RSA file is included and enter the password provided.

##Required Changes Made
1.  installed apache, postgresSQL, mod_wsgi, git, and all required files for catalog app
2.  configured firewall to block all ports other than 2200, 123, and 80
3.  set timezone to UTC
4.  changed SSH port to 2200
5.  added user grader, enabled sudo
6.  added user catalog, set up with limited permissions with psql

##Additional Configurations Made
1. cron scripts to automatically manage package updates
2. ntp time server change to US pool zone
