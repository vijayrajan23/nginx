FROM nginx
RUN mkdir -p /var/www/redis/html
COPY ./redis/web/redis/ /var/www/redis/html/
RUN unlink /etc/nginx/conf.d/default.conf
COPY ./redis/conf/redis.conf /etc/nginx/conf.d/
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]