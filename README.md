# LinuxServerConfiguration

This is my submission for the Udacity Linux Server Configuration project

## Server details

IP Address: 35.178.149.161
URL: http://corinnescatalog.35.178.149.161.xip.io/genres

## Software Installed

Finger
pip
Flask
oauth2client
flask-httpauth
sqlalchemy
Flask-SQLAlchemy
psycopg2-binary
requests
postgresql, postgresql -contrib
mod_wsgi
apache2
httplib2

## Configurations made

### Users

User `grader` added to sudoer.d file to give sudo privileges.
User `ubuntu` added as postgrs superuser that can interact with library database, password protected.

### Security

Ports listening on 2200, 80 and 123.
Users can only login with public/private keys
Login not possible with `root`
Database authentication changed from `peer` to `md5`

### Web server

VirtualHost file configured to serve Public IP address as above with ServerAlias of URL given above.

### Resources

* [Apache VirtualHost Examples](https://httpd.apache.org/docs/2.4/vhosts/examples.html)
* [Using xip.io](https://www.getmura.com/blog/wildcard-dns-using-xipio/)
* [Understanding Peer Authentication](https://stackoverflow.com/questions/18664074/getting-error-peer-authentication-failed-for-user-postgres-when-trying-to-ge)
* [Help understanding how to configure wsgi file only](https://github.com/harushimo/linux-server-configuration)
* [Creating users on Postgrsql](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-16-04)




