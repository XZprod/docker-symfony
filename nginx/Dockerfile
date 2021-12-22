FROM nginx:stable-alpine
RUN apk add --no-cache bash
RUN rm /etc/nginx/conf.d/default.conf
COPY conf.d/*.conf /etc/nginx/conf.d/
WORKDIR /srv/app