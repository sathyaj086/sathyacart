#This is dockerfile cart frontend 
#DOCKERACTION command
FROM index.docker.io/centos:7
MAINTAINER mohanraz@gmail.com
RUN yum -y update
RUN yum -y install httpd php php-gd php-mysql
ENV MY_DB_HOST_WRITE=test MY_DB_HOST_READ=test MY_DB_NAME=test MY_DB_USER=test MY_DB_PASS=test
ADD code /var/www/html
EXPOSE 80
CMD ["/usr/sbin/apachectl", "-D", "FOREGROUND"]