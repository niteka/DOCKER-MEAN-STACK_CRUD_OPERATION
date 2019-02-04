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

```