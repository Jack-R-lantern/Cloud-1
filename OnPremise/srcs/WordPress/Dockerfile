# Base
FROM alpine:3.15

# apk update & install
RUN apk update && \
	apk add --no-cache php8 php-fpm

# WordPress install
ADD https://ko.wordpress.org/latest-ko_KR.tar.gz /var/www/
RUN	cd /var/www && tar -xzvf latest-ko_KR.tar.gz && \
	rm -f latest-ko_KR.tar.gz


CMD php -S 0.0.0.0:80 -t /var/www/