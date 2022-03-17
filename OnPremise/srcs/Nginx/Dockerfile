# Base
FROM alpine:3.15

# apk update & install
RUN apk update && \
	apk add --no-cache openssl && \
	apk add --no-cache nginx

# container run cmd
CMD ["nginx", "-g", "daemon off;"]