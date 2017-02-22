#Project: Linux Server Configuration

##The Amazon Lighsail Server IP: 54.197.142.250

A aws lighsail server(full-stack-server) was created for this project with public accessable IP address 54.197.142.250.

##How to ssh to the server
* The server is listening on port 2200 for ssh.
* a user 'grader' was added to the server for testing.
* please find the private keys in 'ssh' folder for ssh public-key connection. There are two private keys('graderPrivateKey.pem' for Openssh compatible clients, 'graderPrivateKey.ppk' for putty client.)
* After ssh into the server with user 'grader', run 'sudo -s' to be 'root' and execute administrative commands.

## The Web Application Server
* The apache2, mod_wsgi, flask application(Item Catalog) and Postgresql were installed and configured for hosting the project 5-Item Catalog application on the TCP port 80(www).
* Open the url 'http://54.197.142.250' in the browser can access to the web application.