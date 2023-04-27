FROM alpine


RUN apk update
RUN apk add apache2 
#coping my html file in container
COPY mytest.html /var/www/localhost/htdocs/
#changed to done in html conf file as #ServerName www.example.com:80 to ServerName localhost

COPY httpd.conf /etc/apache2/httpd.conf       

EXPOSE 80
CMD [ "httpd", "-D", "FOREGROUND" ]
