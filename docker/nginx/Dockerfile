# Create a Nginx image.
ARG REGISTRY=""
ARG REPOSITORY=""
FROM ${REGISTRY}${REPOSITORY}golden-nginx:latest AS f4rside-site

ARG BUILD_TAG=local
LABEL build_tag=${BUILD_TAG}
LABEL description="The F4rside site"

# Create a folder to serve the public files from.
WORKDIR /srv

# Use a custom Nginx configuration.
COPY docker/nginx/nginx.conf /etc/nginx/conf.d/default.conf

# Copy the f4rside-site distribution files.
COPY src/ /srv/
