FROM nginx
RUN mkdir -p /var/www/one/html
COPY ./one/web/one/* /var/www/one/html
RUN unlink /etc/nginx/conf.d/default.conf
COPY ./one/conf/one.conf /etc/nginx/conf.d/
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]