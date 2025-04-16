FROM node:20.9.0-alpine3.18
RUN adduser -D sodre
WORKDIR /app
COPY package*.json .
RUN npm install
COPY . .
EXPOSE 8080
ENTRYPOINT [ "node", "server.js"]
USER sodre
