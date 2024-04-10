FROM nginx

# Remove the default nginx index.html file
RUN rm -rf /usr/share/nginx/html/index.html

# Remove the default nginx configuration files
RUN rm -rf /etc/nginx/nginx.conf 
RUN rm -rf /etc/nginx/conf.d/default.conf

# Copy your custom nginx configuration
COPY roboshop.conf /etc/nginx/nginx.conf

# Copy your static files to the nginx HTML directory
COPY static /usr/share/nginx/html/

