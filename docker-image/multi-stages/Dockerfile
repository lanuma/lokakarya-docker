FROM node:lts AS build

WORKDIR /app

ADD src/ /app

RUN npm install

FROM node:alpine

ENV NODE_ENV="production"

COPY --from=build /app /app

WORKDIR /app

EXPOSE 3000

ENTRYPOINT ["./bin/www"]
