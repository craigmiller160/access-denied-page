FROM nexus-docker-craigmiller160.ddns.net/nginx-base:1.1.3

RUN mkdir -p /var/www/cert
COPY nginx.conf /etc/nginx/nginx.conf
COPY ../src/index.html /var/www
COPY ../src/index.css /var/www

ENTRYPOINT ["nginx","-g","daemon off;"]