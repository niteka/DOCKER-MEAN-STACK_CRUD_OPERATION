#Dockerfile For Front End
#Linux distribution designed for power users who appreciate security, simplicity and resource efficiency and small
FROM node:alpine
## install, upgrade on running
RUN apk update && apk add
#creating a new directory
RUN mkdir -p /usr/src/app 
# working directory inside the Container
WORKDIR /usr/src/app
#copying the ‘package.json’ file from our project directory to inside the container.
COPY package.json /usr/src/app
#cleans the npm cache
RUN npm cache verify
###installs any packages that it depends on
RUN npm install 
# copy all the codes, folders present from the project directory to inside the container.
COPY . /usr/src/app
# asks the container to expose port number 5555 for communicating with back end server to send requests made by users accessing the front end client via the Web UI.
EXPOSE 5555
# starts executing the codes for building our Angular app.
CMD /usr/src/app/node_modules/\@angular/cli/bin/ng server --host 0.0.0.0 --port 5555









