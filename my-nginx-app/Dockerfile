# Use the official Nginx base image
FROM nginx:latest

# Remove the default Nginx configuration file
RUN rm /etc/nginx/conf.d/default.conf

# Copy your custom Nginx configuration file
COPY nginx-default.conf /etc/nginx/conf.d/default.conf

# Copy your custom HTML files
COPY html /usr/share/nginx/html

# Expose port 80 (default HTTP port)
EXPOSE 80

# Nginx starts automatically when the container runs due to the base image's CMD
