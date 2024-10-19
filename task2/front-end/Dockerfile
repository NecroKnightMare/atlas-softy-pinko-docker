# latest version of nginx
FROM nginx:latest

# Copy to frontend
COPY . /var/www/html/softy-pinko-front-end

# Copy to image
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
