# docker-uni-example

### It is a University project for the show the base capabilities of Docker.

**Cheatsheet commands:** 

- **docker info** - display system information

- **docker ps** - list running containers *if we add the option -a will list all containers*

- **docker run ubuntu /bin/echo 'Hello world'** - create a new container using the ubuntu image and write on terminal "Hello world"

- **docker build -t test-python .** - create a new image named test-python based on the ***Dockerfile***

- **docker images** - display all local images

- **docker run -p 4000:80 test-python** - run the test-python image (built previous) and mapping the host port *4000* to the container port *80* 
*if we add the option -d  the container will run in background*

- **docker-compose up** - start and configure the containers based on the ***docker-compose.yml*** file

- **docker rm $(docker ps -a -q)** - stop all containers and remove them


This example is created based on Docker documentation: https://docs.docker.com/get-started/
