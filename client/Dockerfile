FROM node:current-alpine3.17

#setting my working directory for the commands to be run on
WORKDIR /usr/src/app

COPY package*.json /usr/src/app/


#install dependencies from both package files
RUN npm ci

COPY . .


#telling docker which port to listen to during runtime
EXPOSE 3000

CMD ["npm","start"]