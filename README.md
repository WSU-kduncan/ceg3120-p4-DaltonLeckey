Part 1: Dockerize it

Using the information in https://hub.docker.com/_/httpd 
I got the website up and running locally as seen here: 

the commands used were: 
$ docker build -t my-apache2 .
$ docker run -dit --name my-running-app -p 8080:80 my-apache2

Part 2: Github Actions

Set up the workflow and using the course video and the link provided 
I set everything up using the template provided.

Part 3: Dockerhub Documentation