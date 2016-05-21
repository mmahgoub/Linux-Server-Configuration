# Linux Server Configuration
Installation of a Linux distribution on a virtual machine and prepare it to host a web applications, include installing updates, securing it from a number of attack vectors and installing/configuring web and database servers.

## Server Information
- Domain name: http://catalog.mmahgoub.com (To enable Google login)
- IP address: 52.39.232.171
- SSH port: 2200

## Summary
- Created a new user named "grader"
- Gave the grader the permission to sudo
- Updated all currently installed packages
- Changed the SSH port from 22 to 2200
- Configured UFW to only allow incoming connections for SSH (port 2200), HTTP (port 80), and NTP (port 123)
- Configured the local timezone to UTC
- Installed and configured Apache to serve a Python mod_wsgi application
- Installed and configure PostgreSQL:
- Configured PostgreSQL to deny remote connections
- Created a new user named catalog that has limited permissions to your catalog application database
- Installed git and cloned my Catalog App project (https://github.com/mmahgoub/fullstack-nanodegree-vm/tree/master/vagrant/catalog)
- Installed PIP
- Configured Apache virtual hosts
- Installed required python modules via PIP
- Made some changes to Catalog App required to run Flask with Apache

## Resources
- [How To Deploy a Flask Application on an Ubuntu VPS](https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps)
- [SQLAlchemy - DBAPI Support](http://docs.sqlalchemy.org/en/latest/dialects/postgresql.html#module-sqlalchemy.dialects.postgresql.psycopg2)
- [Ubuntu PostgreSQL Community Page](https://help.ubuntu.com/community/PostgreSQL)
