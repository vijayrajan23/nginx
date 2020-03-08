FROM nginx
RUN mkdir -p /etc/nginx/ssl-certs
COPY ./gate/ssl-certs/* /etc/nginx/ssl-certs/
RUN unlink /etc/nginx/conf.d/default.conf
COPY ./gate/conf/rever.conf /etc/nginx/conf.d/
COPY ./gate/conf/reverone.conf /etc/nginx/conf.d/
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]