FROM node:22.5.1-slim

ENV INSTANA_AUTO_PROFILE true

EXPOSE 8080

WORKDIR /opt/server

COPY package.json /opt/server/

RUN npm install

COPY server.js /opt/server/

CMD ["node", "server.js"]

