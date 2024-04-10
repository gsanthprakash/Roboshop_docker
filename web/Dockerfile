FROM nginx:latest
RUN rm -rf /usr/share/nginx/html/index.html
RUN rm -rf /etc/nginx/nginx.conf
RUN rm -rf /etc/nginx/conf.d/default.conf
COPY roboshop.conf /etc/nginx/nginx.conf
ADD static /usr/share/nginx/html/
EXPOSE 8080
CMD ["nginx", "-g", "daemon off;"]