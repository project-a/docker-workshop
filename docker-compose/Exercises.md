# Some exercises to practice

Tip: the [official documentation of the used Docker images](https://hub.docker.com/_/nginx) most often contains 
instructions on where to place files needed for the configuration of the Docker containers

1. Take the nginx container from the Example folder, attach the bash to it and create a custom `index.html` file 
to display when connecting to the container port

2. Create the `index.html` file outside the container and mount it into the container via `docker-compose.yml` configuration

3. Expose the Nginx server so that only other containers can communicate with it and it's not reachable from outside
(you can test this by connecting to the DB container and using `curl`... not installed by default!)

4. Connect to the MySQL container with a DB client: it's empty. Follow the documentation of the Docker image so that 
the container executes automatically the scripts found in the `db_scripts` folder to bootstrap some data in the DB schema.