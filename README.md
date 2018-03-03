# postgresql



how to install postgresql in ubuntu 16.04 there two way to install 



one is simple if it's don't ask to dependency


</br>sudo add-apt-repository "deb http://apt.postgresql.org/pub/repos/apt/xenial-pgdg main"

</br>wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -
</br>
</br>sudo apt-fast -y install postgresql-10
</br>sudo apt-get install postgresql-common
</br>sudo apt-get install postgresql-server-dev-all

</br>
then create super user using this command
</br>
sudo su - postgres
createuser -s #yourname



second method if it's won't work then we have install in different way


sudo vim /etc/apt/sources.list


Add this to your sources.list:
</br>
</br>deb http://ftp.de.debian.org/debian/ wheezy main non-free contrib
</br>deb-src http://ftp.de.debian.org/debian/ wheezy main non-free contrib

Make sure you use the appropriate mirror for your location.

Run aptitude update or apt-get update and finish the installation.

The interactive mode of aptitude is quite useful to solve dependencies.





</br>apt-get install ssl-cert

</br>sudo apt-fast -y install postgresql-10



</br>sudo vim /etc/apt/sources.list.d/pgdg.list

</br>
</br>deb http://apt.postgresql.org/pub/repos/apt/ xenial-pgdg main

</br>deb http://apt.postgresql.org/pub/repos/apt/ precise-pgdg main



