# syntax=docker/dockerfile:1
FROM alpine:3.19
ENV NODE_VERSION 22.5.1
ENV NODE_ENV=production

WORKDIR /app

COPY ["package.json", "package-lock.json*", "./"]

RUN npm install --production

COPY . .

EXPOSE 8080
CMD [ "node", "server.js" ]
