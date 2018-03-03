# postgresql



how to install postgresql in ubuntu 16.04 there two way to install 



one is simple if it's don't ask to dependency


sudo add-apt-repository "deb http://apt.postgresql.org/pub/repos/apt/xenial-pgdg main"
wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -

sudo apt-fast -y install postgresql-10
sudo apt-get install postgresql-common
sudo apt-get install postgresql-server-dev-all


then create super user using this command

sudo su - postgres
createuser -s #yourname



second method if it's won't work then we have install in different way


sudo vim /etc/apt/sources.list


Add this to your sources.list:

deb http://ftp.de.debian.org/debian/ wheezy main non-free contrib
deb-src http://ftp.de.debian.org/debian/ wheezy main non-free contrib

Make sure you use the appropriate mirror for your location.

Run aptitude update or apt-get update and finish the installation.

The interactive mode of aptitude is quite useful to solve dependencies.





apt-get install ssl-cert

sudo apt-fast -y install postgresql-10



sudo vim /etc/apt/sources.list.d/pgdg.list


deb http://apt.postgresql.org/pub/repos/apt/ xenial-pgdg main

deb http://apt.postgresql.org/pub/repos/apt/ precise-pgdg main



