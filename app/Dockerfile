# syntax=docker/dockerfile:1

FROM  node:18.19.1-bullseye-slim 
ENV NODE_ENV=production

WORKDIR /app

COPY ["package.json", "package-lock.json*", "./"]

RUN npm install --production

COPY . .

EXPOSE 8080
CMD [ "node", "server.js" ]
