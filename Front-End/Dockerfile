FROM node:8-alpine
COPY . /app
WORKDIR /app
RUN npm config set proxy=http://web-proxy.in.hpecorp.net:8080 && npm install
EXPOSE 4000
CMD ["node", "server.js"]
