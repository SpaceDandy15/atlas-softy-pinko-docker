# Use the latest version of Nginx
FROM nginx:latest

# Copy the front-end files to the Nginx HTML directory
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy the Nginx config file to the appropriate directory
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# Expose port 9000 to the host
EXPOSE 9000
