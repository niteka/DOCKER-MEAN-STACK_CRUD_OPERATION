
#Dockerfile For Back End
#alpine Linux distribution designed for power users who appreciate security, simplicity and resource efficiency and small
FROM node:alpine
# install, upgrade on running
RUN apk update && apk add
#creating a new directory
RUN mkdir -p /usr/src/app 
# working directory inside the Container
WORKDIR /usr/src/app
#copying the ‘package.json’ file from our project directory to inside the container.
COPY package.json /usr/src/app
#Verify the contents of the cache folder, garbage collecting any unneeded data, and verifying the integrity of the cache index and all cached data.
RUN npm cache verify
#installs any packages that it depends on
RUN npm install
# copy all the codes, folders present from the project directory to inside the container.
COPY . /usr/src/app
# asks the container to expose port number 3000 for communicating with back end server to send requests made by users accessing the front end client via the Web UI.
EXPOSE 3000
# starts executing the codes for building our Angular app.
CMD ["node","index.js"]