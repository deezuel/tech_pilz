FROM nginx:latest

RUN apt-get update && apt-get upgrade -y

VOLUME [ "/etc/nginx", "/usr/share" ]

COPY index.html /usr/share/nginx/html

COPY default.conf /etc/nginx/conf.d

EXPOSE 8080

