FROM httpd
RUN apt-get update && apt-get install -y \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/* \
    mkdir /usr/local/apache2/conf/extra
COPY conf/httpd.conf /usr/local/apache2/conf/httpd.conf
COPY conf/httpd-proxy.conf /usr/local/apache2/conf/extra/httpd-proxy.conf
EXPOSE 80
