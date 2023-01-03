FROM node:lts-alpine

RUN apk add bash

WORKDIR /app
COPY . .
RUN npm ci

EXPOSE 3000
ENTRYPOINT ["npm", "run", "start:prod"]
