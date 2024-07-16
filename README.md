# AWS-Project

# This helps to deploy the source code into webserver automatically
version: 0.0
os: linux
files:
 - source: /index.html
   destination: /var/www/html
hooks:
 BeforeInstall:
 - location: scripts/httpd_install.sh
   timeout: 300
   runas: root
 - location: scripts/httpd_start.sh
   timeout: 300
   runas: root
ApplicationStop:
 - location: scripts/httpd_stop.sh
   timeout: 300
   runas: root
