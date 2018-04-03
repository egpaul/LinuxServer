# LinuxServer
Udacity FSND Linux Server Configuration 

## Server Acceess 

~~* IP Address 54.89.126.77~~
~~* ssh -i ~/.ssh/linuxProject grader@54.89.126.77 -p 2200~~

* Project has been completed. Lightsail server is no longer active. 

## Software/libs installed

* Apache 2
* Flask
* Finger
* httplib2
* oauth2
* Postgree
* psycopg2
* Python 2.7
* pip
* sqlalchemy
* requests

## Configurations Made

* Set up of virtual Machiene on Amazon Lightsail
* Update/upgrade all installed packages
  * Update installed packages by running `sudo apt-get update` and then `sudo apt-get upgrade`
* Update timezone to UTC
  * Update timezone by `sudo dpkg-reconfigure tzdata` select `none of the above` and then `UTC`
* Creation of a new user "grader" 
  * `sudo adduser grader`. Fill out the details when asked
* Change port from 22 to 2200
  * `sudo nano /etc/ssh/sshd_config` Locate "Port 22" and change to Port 2200"
  * Restart SSH `sudo service ssh restart`
* Configured UFW to only allow allow incoming connections for SSH(Port:2200), HTTP(Port:80) and NTP(Port:123)
  * `sudo ufw allow 2200`, `sudo ufw allow 80`, `sudo allow 123`
  * Enable UFW `sudo ufw enable`
* Installed Apache server and Python 
  * `sudo apt-get install apache2 libapache2-mod-py`
  * `sudo apt-get install python`
* Configured Apache server to run python wsgi mods
  * Create the wsgi conf file `sudo nano /etc/apache2/sites-available/catalog.conf`
* Installed and configured PostgreSQL
  * `sudo apt-get install postgresql`
* Created "catalog" user in PostgreSQL

