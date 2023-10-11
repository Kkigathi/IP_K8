FROM node:20-alpine3.17

COPY package*.json /app/

#setting my working directory for the commands to be run on
WORKDIR /app

#install dependencies from both package files
RUN npm install


#telling docker which port to listen to during runtime
EXPOSE 3000

CMD ["npm","start"]