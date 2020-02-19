# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent
EXPOSE 8080
RUN sed -i "s/Listen 80/Listen 8080/g" /etc/httpd/conf/httpd.conf
RUN chgrp -R root /var/log/httpd /var/run/httpd && 
    chmod -R g=u /var/log/httpd /var/run/httpd
USER 1001

