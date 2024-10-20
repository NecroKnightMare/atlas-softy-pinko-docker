# latest version of nginx and nginx dir
FROM docker.io/library/nginx:latest@sha256:af296b188c7b7df99ba960ca614439c99cb7cf252ed7bbc23e90cfda59092305
# Copy to frontend
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end
# Copy to image
COPY ./softy-pinko-front-end.conf  /etc/nginx/conf.d/default.conf