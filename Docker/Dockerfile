FROM ubuntu

RUN apt-get -y update && \
    apt install -y nginx && \
    apt install -y curl && \
    apt install -y vim

WORKDIR meu-site

COPY index.html /var/www/html
COPY Docker.png /var/www/html

LABEL Image="Imagem do ronald" \
    Author="Ronald" \
    Version="1.0" \
    Description="Imagem do ronald" \
    E-mail="rm552364@fiap.com.br"

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]