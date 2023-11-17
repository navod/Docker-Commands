# Docker-Commands
Basic docker commands

What is contaner?

* Lightweight, standalone and executable software package that includes everything needed to run a peace of software.
* Containers are designed to provide a consistent are repoducible environment accross different platforms are development stages.
* Simplifies development, deployment and scaling.

Containers benifits
* Consistency
* Portability
* Resource Efficiency
* Scalability
* Versioning and Rollback

What are containers?
* Containers Repository
* Private Repositories
* Public Repository

Virtual Machine and Docker Container
--------------------------------------
##todo

What is docker container?
--------------------------
##todo

Check Docker version -
# docker -v

How to pull container?
# docker pull postgres

![image](https://github.com/navod/Docker-Commands/assets/66496106/a503d220-416e-4461-bab5-39973db4d86e)

Two ways to check docker images

# docker images

How to run docker?

1. docker run <image_name>
2. docker run -d <image_name> (-d means detach mode)

After getting this error run this code 
# docker run -e POSTGRES_PASSWORD=password postgre
 How to find what are the running docker containers
 docker ps

How to stop running
docker stop <container_id>

How to load and all containers (running/stop) (-a means all)
docker ps -a 

Each time you execut docker run command it will create a new docker container


Docker Architecture
-------------------
##todo

How to run same container without creating new container
docker start <container_id>

how to find logs
docker logs <docker_name>

Keep listing logs
docker logs -f sweet_sanderson

How to go to inside docker container
docker exec -it <container_name> psql -U postgres
exec - execute
-it - internal terminal
psql - postgresql
-U - User
postgres - username

how to exit the containr
exit

how to customize container name when running container (-e means enviorenment)
docker run --name <customise_name> -e POSTGRES_PASSWORD=password postgres

how to run docker container on detach mode ( -d means detach)
docker run -d --name <customize_name> -e POSTGRES_PASSWORD=password postgres

how to remove docker container
docker rm <container_id>
rm - remove

how to remove docker image
docker rmi <image_id>
rmi - removde image id

How to pull specific image versions
docker pull redis:6.2


