FROM nginx:latest

WORKDIR /nginx

RUN chown nginx:nginx /nginx
RUN chown nginx:nginx /var/cache/nginx/
USER nginx

COPY ./data /nginx/data
COPY ./conf /nginx/conf

CMD ["nginx", "-c", "/nginx/conf/nginx.conf"]
