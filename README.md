#Project: Linux Server Configuration

##The Amazon Lighsail Server IP: 54.197.142.250

A aws lighsail server(full-stack-server) was created for this project with public accessable IP address 54.197.142.250.

##How to ssh to the server
* The server is listening on port 2200 for ssh.


## The Web Application Server
* Open the url 'http://54.197.142.250' in the browser can access to the web application.

## Software Installed and Changes Made
* Installed Softwares for this project:
  * Apache2
  * libapache2-mod-wsgi
  * postgresql
  * python-psycopg2
  * python-sqlalchemy
  * python modules(pip) : werkzeug, flask, Flask-Login, oauth2client, requests, httplib2

* a user 'grader' was added to the server for testing.
* After ssh into the server with user 'grader', run 'sudo -s' to be 'root' and execute administrative commands.
* Linux firewall rules only allow TCP/2200, TCP/80, UDP/123 for incoming access.
* the Flask Application was cloned from github(https://github.com/ldwang/FSWDND-P5-Item-Catalog) to '/var/www/catalog'.
* The postgresql server is running only on localhost:5432.
* A database user 'catalog' was granted to full privileges to database 'catalog'. user 'catalog' can connect to 'localhost/catalog' without password.
* The sqlalchemy engine was modified to connect to postgresql catalog database.
* the apache2 configuration file '/etc/apache2/sites-enabled/000-default.conf' was changed to support the mod-wsgi '/var/www/catalog/catalog.wsgi'. 

 ## Third party resources
 * https://github.com/ldwang/FSWDND-P5-Item-Catalog
 * http://www.jakowicz.com/flask-apache-wsgi/
 * http://flask.pocoo.org/docs/0.12/deploying/mod_wsgi/
 
 ## SSH keys
 The SSH keys is under '/home/grader/ssh_key_grader' folder. 
 * "id_rsa" - private key
 * "id_rsa.pub" - public key.
 
 The 'grader' user's SSH key will be pasted into the 'Notes to Reviewer' field during the submission process.