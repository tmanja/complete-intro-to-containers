FROM node:12-alpine

USER node

RUN mkdir /home/node/code

WORKDIR /home/node/code

COPY --chown=node:node . .

RUN npm ci

EXPOSE 3000

CMD [ "node", "index.js" ]
