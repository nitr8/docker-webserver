FROM alpine:3.5

RUN apk add --update nginx && rm -rf /var/cache/apk/*

ADD nginx.conf /etc/nginx/nginx.conf

RUN mkdir /www
#RUN mkdir /errors
#ADD error_pages /errors
ADD www /www

EXPOSE 80

CMD ["nginx"]
