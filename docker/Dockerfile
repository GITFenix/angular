FROM debian:stretch
WORKDIR /var/www/angular

RUN apt-get update && apt-get install -y curl git gnupg2
RUN curl -sL https://deb.nodesource.com/setup_11.x | bash - && apt-get install -y nodejs
RUN npm install -g @angular/cli

CMD [ "ng", "serve", "--host=0.0.0.0", "--port=80", "--disable-host-check"]
