FROM nginx:latest
RUN rm -rf /usr/share/nginx/html/*
COPY roboshop.conf /etc/nginx/conf.d/roboshop.conf
ADD static /usr/share/nginx/html/static
EXPOSE 8080
CMD ["nginx", "-g", "daemon off;"]