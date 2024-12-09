FROM node:20.18.1-alpine
WORKDIR /app
# otimização de cache, roda o npm install apenas se o package.json mudar
COPY package*.json .
RUN npm install
COPY . .
EXPOSE 8888
CMD ["node", "server.js"]