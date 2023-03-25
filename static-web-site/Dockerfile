FROM amazonlinux:latest
LABEL name="suraj-singh"
RUN yum install -y httpd \
         zip \
        unzip
ADD https://www.free-css.com/assets/files/free-css-templates/download/page289/zon.zip /var/www/html
WORKDIR /var/www/html
RUN unzip zon.zip
RUN cp -r zon-html/. . 
CMD ["/usr/sbin/httpd", "-D" ,"FOREGROUND"]
