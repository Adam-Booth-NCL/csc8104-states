FROM node:22-alpine

WORKDIR /usr/src/states

COPY package.json .

RUN npm install --omit=dev

COPY server.js db.json ./

EXPOSE 8080

CMD [ "node", "server.js" ]
