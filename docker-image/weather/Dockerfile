FROM node:lts

# git clone https://github.com/linuxacademy/content-weather-app.git src

WORKDIR /app

ADD src/ /app/

RUN npm install

EXPOSE 3000

CMD ./bin/www
