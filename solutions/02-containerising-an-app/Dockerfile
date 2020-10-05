# use node LTS (12.x), alpine linux distro
FROM node:erbium-alpine

# need port 3000 open for our application to receive requests on
EXPOSE 3000

# use node user for security purposes
USER node
RUN mkdir /home/node/app
WORKDIR /home/node/app

# copy over package config and install deps
COPY --chown=node:node package-lock.json package.json ./
RUN npm ci

# copy over rest of files
COPY --chown=node:node . .

# run service by default
CMD ["node", "server.js"]