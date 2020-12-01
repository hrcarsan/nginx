# docker build -t hrcarsan/nginx:1.10-nr .
FROM nginx:1.10.3-alpine

RUN set -x \
	&& addgroup -g 82 -S www-data \
	&& adduser -u 82 -D -S -G www-data www-data \
  && chown -R www-data: /var/cache/nginx \
  && chown -R www-data: /var/run

USER www-data
