# LinuxServerConfig

ssh port: 2200  
ip address: 54.200.7.7  
Host name: http://54.200.7.7.xip.io  

# Setup  
Installed Apache `sudo apt-get install apache2`  
Installed mod_wsgi `sudo apt-get install libapache2-mod-wsgi python-dev`  
Install virtual environment `sudo apt-get install python-pip` then `sudo pip install virtualenv`  
Install Flask and other dependencies `sudo pip install Flask`  
Cloned app repo into server using git `apt-get install git-core` then `git clone https://github.com/brewso/Catalog`  
Created new apache site availible `sudo nano /etc/apache2/sites-available/appwsgi.conf`  
Activated new site `sudo a2ensite appwsgi`  
Deactivate default site  `sudo a2dissite 000-default`  
Found and fixed any errors by referencing apache error.log

Used [this tutorial](https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps)  
Fixed some issues referencing [here](https://modwsgi.readthedocs.io/en/develop/user-guides/application-issues.html#application-working-directory)  
