1. base image: node:20-alpine3.17
    the base image version was selected as it is a lightweight linux based node image.
2.docker file directives used
    --COPY-- was initially used so as to give the container i want to build from the image the required files it needed, so as to download all its dependencies
    the flag "*" just specifies to copy all files with "package---" name and json extension
    
    --WORKDIR-- sets a specified directory in the container to be the one in which all underlying commands will be executed on.

    --RUN-- RUNS a specified command of which in my case was to install dependencies, specified in the package.json files

    --expose-- specifies to docker which port to listen to once the container goes live

    --CMD-- specifies the default executable of my docker image.

--Docker volume-- the convention is used for teh docker volume was to name it after the Database name specifed in the code i.e yolomy
