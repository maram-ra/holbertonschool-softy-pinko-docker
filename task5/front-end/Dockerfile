# Use Nginx as the base image
FROM nginx:latest

# Copy static files to Nginx default directory
COPY . /var/www/html/softy-pinko-front-end

# Copy custom Nginx config
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
