# practising-docker
To play-around with docker

#### About Project
This is a simple project with a basic Dockerfile to build a python app.

#### Building and Pushing Image to docker hub
You can build the image manually by running 

`docker build -t psaini0212/practicing-docker .`

and then you can push this to docker hub - practicing-docker repository.

`docker push psaini0212/practicing-docker`

Though this project is connected to docker hub to build images automatically 
which means any push to this repo with trigger a build automatically in 
docker hub and will build a new image with tag latest.

Check this 


https://cloud.docker.com/repository/docker/psaini0212/practising-docker/builds

#### Docker Compose

In  a docker compose file - you can define how your containers will behave in production.

```
docker init swarm
docker stack deploy -c docker-compose.yml getstarted_lab
docker stack ls
docker service ls
docker service ps getstarted_lab_web
docker stack rm getstarted_lab
```

