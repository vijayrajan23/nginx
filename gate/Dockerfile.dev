FROM nginx
RUN mkdir -p /etc/nginx/ssl-certs
COPY ssl-certs/* /etc/nginx/ssl-certs/
RUN unlink /etc/nginx/conf.d/default.conf
COPY conf/rever.conf /etc/nginx/conf.d/
COPY conf/reverone.conf /etc/nginx/conf.d/
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]