# Base on offical NGINX Alpine image
FROM nginx:alpine

# Remove any existing config files
RUN rm /etc/nginx/conf.d/*

# Copy config files
# *.conf files in conf.d/ dir get included in main config
COPY ./http.conf /etc/nginx/conf.d/
# COPY ./etc /etc

# Launch NGINX
CMD [ "nginx", "-g", "daemon off;" ]