# Linux Server Setup and Configuration
## Access the server
- **Server IP address:** 178.128.37.166
- **SSH port:** 2200
- **Address of hosted itemcatalog application:** http://178.128.37.166.xip.io/

## Software Installed
- Apache server software
- Mod_wsgi
- Postgresql was installed but not used
- Git

## Database
Sqlite is used for the database and the database instance can be found in
home/rukykf/itemcat/venv/var/itemcatalog-instance

All the files for the itemcatalog application can be found in 
home/rukykf/itemcat/venv/lib/python2.7/site-packages/itemcatalog
The database configuration for the itemcatalog app is in the __init__.py file in the itemcatalog folder. 

## Configuration changes made
- UFW was used to only allow traffic for HTTP, SSH and NTP
- Login with password is disabled on the server, users must login with their private key
- Login as root is disabled on the server
- SSH port was changed from the default to port 2200
