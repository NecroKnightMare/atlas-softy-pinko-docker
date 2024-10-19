# latest version of nginx
FROM nginx:latest

# Copy to frontend
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy to image
COPY softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# expose port for continuous error
EXPOSE 9000