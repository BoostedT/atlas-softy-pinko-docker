# Use the latest version of nginx as the base image
FROM nginx:latest

# Copy the softy-pinko-front-end files to the Nginx HTML directory
COPY softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy the Nginx configuration file to the default location
COPY softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf