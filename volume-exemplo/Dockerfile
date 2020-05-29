FROM node:latest
LABEL maintainer="Luiz Henrique de Souza | luizhsou1@gmail.com"
LABEL version="0.1"
LABEL description="This is custom Docker Image for Node.js"
ENV NODE_ENV=production
ENV PORT=3000
COPY . /var/www
WORKDIR /var/www
RUN npm install
ENTRYPOINT [ "npm", "start" ]
EXPOSE $PORT