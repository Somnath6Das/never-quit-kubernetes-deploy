// build docker image
docker build -t hello-docker .

// to see image list
docker image ls

// run docker image
docker run hello-docker

// login to docker hub
docker login

// push to docker hub
docker tag hello-docker:latest somnath8das/hello-docker
docker push somnath8das/hello-docker

// remove docker image
docker rmi somnath8das/hello-docker

// download image from docker hub
docker pull somnath8das/hello-docker

// to run image
docker run somnath8das/hello-docker

// to run node app on port
docker run -p 4000:4000 somnath8das/hello-docker
