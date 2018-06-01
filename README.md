# linux_server_configuration
Final project for Udacity's FSND Project 5. Describes how to configure a Linux server and deploy a Python Flask web app with a PostgreSQL backend to AWS. 

    IP Address: 35.182.227.203
    SSH Port: 2200
    Url: 35.182.227.203.xip.io

    To log into server:
    ssh grader@35.182.227.203 -p 2200 -i ~/.ssh/id_rsa

### Summary of Software Installed

- Python mod_wsgi
- Apache2
- PostgreSQL
- Git
- Virtual Environment (virtualenv)
- Python pip
- Flask
- Catalog App dependencies
    - sqlalchemy
    - psycopg2 (python-psycopg2)
    - oauth2client
    - httplib2
    - requests

### Summary of Configurations Made:

- New user 'grader' added, given sudo permission
- Key-based Authentication/Public Key encryption setup for grader & public key added to server
- Set up permissions for grader
- Password based login disabled (key pair login required)
- Disabled remote login of the root user
- Changed ssh port from 22 to 2200
- Configured firewall to only allow incoming connections for SSH (port 2200)
- Configure local timezone to UTC
- Install and configured Apache to serve a Python mod_wsgi application
- Installed and configured Postgresql
- Created a new database user with limited database permissions
- Installed Git and cloned previous Udacity project 3 from Full Stack Nanodegree to this server
- Installed Flask and created a Virtual Environment for project 3
- Added any additional software for the Application
- Updated OAuth information for Google login

Special Thanks to [twhetzel](https://github.com/twhetzel) for a very helpful [README](https://github.com/twhetzel/ud299-nd-linux-server-configuration).
