This python script will ask some informations by terminal prompts to configure folders'names ,databse name,configuration files contents , etc..
then it will generate 4 files :
- sql file : to create database, create user and grant permission on the database to the user
- apache2 conf file : to give webserver access to the owncloud folder
- bash file : to install web server , php and all dependencies to make owncloud works , download owncloud folder archive , extract it, move it to the right place, give him the right owner and permissions , move the apache2 conf file in the right place
, and then restart apache webserver to get the modifications considered
- another bash script that will execute the others

How to proceed : 

-1 : open a terminal and go to the folder where you download the script
-2 : enter the following command : sudo python3 owncloud_easySetup.py
-3 : answer to questions to custom your configuration
-4 : once it's finished enter the following command : sudo ./execute_all_scripts.bash

And once he finished you can now open a browser and go to the url you specified(or local ip adress if there's no DNS registration)
and enter the informations that you entered above to connect your database and ... It's done ! You have now a personnal cloud web-service ;)