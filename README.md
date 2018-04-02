# LinuxServer
Udacity FSND Linux Server Configuration 

## Server Acceess 

* IP Address 54.89.126.77
* ssh -i ~/.ssh/linuxProject grader@54.89.126.77 -p 2200

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
* Update timezone to UTC
* Creation of a new user "grader" 
* Change port from 22 to 2200
* Configured UFW to only allow allow incoming connections for SSH(Port:2200), HTTP(Port:80) and NTP(Port:123)
* Installed Apache server 
* Configured Apache server to run python wsgi mods
* Installed and configured PostgreSQL
* Created "catalog" user in PostgreSQL

