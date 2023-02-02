FROM nexus-docker-craigmiller160.ddns.net/nginx-base:1.1.3

RUN mkdir -p /var/www/cert
COPY ./nginx.conf /etc/nginx/nginx.conf
COPY ./src/index.html /var/www/index.html
COPY ./src/style.css /var/www/style.css
COPY ./cert /var/www/cert

ENTRYPOINT ["nginx","-g","daemon off;"]