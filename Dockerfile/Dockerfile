FROM alpine:latest
RUN \
    apk add --no-cache \
    apache2-proxy \
    apache2-ssl \
    apache2-utils 

WORKDIR /var/www/localhost/htdocs
COPY /tic-tac-toe-game-main/  /var/www/localhost/htdocs 

EXPOSE 80
CMD ["/usr/sbin/httpd", "-D", "FOREGROUND"] 
