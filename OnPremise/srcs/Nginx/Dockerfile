# Base
FROM alpine:3.15

# apk update & install
RUN apk update && \
	apk add --no-cache openssl && \
	apk add --no-cache nginx

# tls setting
RUN mkdir -p /etc/ssl/private && \
 	openssl req -x509 -nodes -newkey rsa:2048  -days 365 \
				-keyout /etc/ssl/private/nginx.key \
				-out /etc/ssl/certs/nginx.crt \
				-subj "/C=KR/ST=SEOUL/O=42Seoul/OU=inception/CN=login.42"

# container run cmd
CMD ["nginx", "-g", "daemon off;"]