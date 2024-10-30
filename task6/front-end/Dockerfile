# Use the latest version of Nginx
FROM nginx:latest

# Copy the front-end files to the Nginx HTML directory
COPY ./softy-pinko-front-end /usr/share/nginx/html/softy-pinko-front-end

# Copy the Nginx config file to the appropriate directory
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# Expose port 80 to the host (Nginx default)
EXPOSE 80
