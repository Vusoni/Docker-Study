FROM node:14

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE $PORT

ARG DEFAULT_PORT=80

ENV PORT 80

# VOLUME [ "/app/node_modules" ]

VOLUME ["/temp"]

CMD [ "npm", "start" ]