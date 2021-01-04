# Create a Nginx image.
FROM nginx:stable-alpine AS test-nginx

EXPOSE 80

# Use a custom Nginx configuration.
COPY docker/nginx/nginx.conf /etc/nginx/conf.d/default.conf
# Create a folder to serve the public files from.
WORKDIR /srv
# Copy the f4rside-site distribution files.
COPY src/ /srv/
