1. Locally connect development mode:

// install mongo container >
docker container run --name mongoc1 -p 5000:27017 -d mongo:6.0.5

// get ip information of mongo container >
docker container inspect mongoC1 

// build node server container >
docker image build -t node-api ./jokes-api

// run node server container >
docker container run --name nodec1 -d node-api

// see container logs >
docker logs <container-id>

2. production level mode:

// create network >
docker network create mern-network

// see all network >
docker network ls

// image run through network >
docker container run --name mongodb --network mern-network -d mongo:6.0.5

// build node server container >
docker image build -t node-api ./jokes-api

// run node container with network
docker container run --name nodec1 --network mern-network -d node-api







