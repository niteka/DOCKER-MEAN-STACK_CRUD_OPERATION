# DOCKER-MEAN-STACK_CRUD_OPERATIONS

## Getting Started

The quickest way to get going is to run:

```sh
docker-compose up --build
```

This will start

- Node server on port [3000](http://localhost:3000)
- MongoDb on port [27017](http://localhost:27017)
- Angular on port [5555](http://localhost:4200) 

Open http://localhost:4200 for front end

### Backup archive files [(for download)](https://we.tl/t-VAxv1l2CHE)
 #### Angular
 - angular-save.tar   | Image size:  489,9 Mo   
 - angular-export.tar  | Container size : 489,1 Mo
 
 #### Node Express
 - node-express-save.tar  | Image size: 94,1 Mo 
 - node-express-export.tar | Container size: 93,7 Mo

#### Mongo
 - mongo-save.tar         | image size: 400 Mo

### Docker Compose

```sh
### Prod ###
# Start all services
docker-compose -f docker-compose.yml up --build

```
## Help

### Docker Commands

```sh
# Stop all running containers
docker stop $(docker ps -aq)

# Remove all containers
docker rm $(docker ps -aq)

# Remove all images
docker rmi $(docker images -q)

# save the image  
docker save image_id > name.tar
# export the container.
docker export container_id > name.tar


```