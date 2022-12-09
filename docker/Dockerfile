FROM node:lts-alpine

RUN apk add bash

WORKDIR /app
COPY . .
RUN npm ci --omit=dev --omit=optional --ignore-script --no-audit --prefer-offline --progress=false

EXPOSE 3000
ENTRYPOINT ["npm", "run", "start:prod"]
