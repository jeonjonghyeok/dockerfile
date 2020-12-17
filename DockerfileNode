FROM node:12.13.0-alpine

RUN apk update && apk add build-base git python

COPY package.json .
COPY yarn.lock .
COPY ./src ./src
COPY ./dist ./dist
COPY ./resources ./resources
COPY ./spec ./spec

RUN yarn install --production

CMD ["yarn", "start:prod"]
