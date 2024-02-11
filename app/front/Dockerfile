# Use a different base image
FROM nginx:alpine

WORKDIR /usr/share/nginx/html

COPY . .

COPY entrypoint.sh /entrypoint.sh

RUN apk add --no-cache bash
RUN chmod +x /entrypoint.sh

EXPOSE 80

ENTRYPOINT ["/entrypoint.sh"]
