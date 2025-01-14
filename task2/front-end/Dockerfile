
# Use latest version of nginx
FROM nginx:latest

# Copy front-end files to Nginx's root directory
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy Nginx config file
COPY softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# Expose port 9000 for the server
EXPOSE 9000
