# This Docker file is for https light-weight image
FROM alpine:latest
RUN apk update && apk add --no-cache apache2
COPY ./index.html /var/www/localhost/htdocs/index.html
COPY ./test-remote-build.txt /var/www/localhost/htdocs/test-remote-build.txt
EXPOSE 80
ENV TEST_ANOSA=Zatona
CMD ["httpd", "-D", "FOREGROUND"]
