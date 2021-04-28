### Part 1: Dockerize it

Using the information in https://hub.docker.com/_/httpd 

**the commands used were:** 

```
$ docker build -t my-apache2 .
$ docker run -dit --name my-running-app -p 8080:80 my-apache2
```

### Part 2: Github Actions

Set up the workflow and using the course video and the link provided
https://docs.github.com/en/actions/guides/publishing-docker-images#publishing-images-to-docker-hub
I set everything up using the template provided.

### Part 3: Dockerhub Documentation

-Installed dockerhub via the link provided, Dockerhub set up all the dependancies needed in installation.

-Used the information provided in part 1, got everything up and running.
![Dockerizing)](https://user-images.githubusercontent.com/77791957/116328600-61f0bf80-a797-11eb-81f1-0a7a5f044619.png)

-Created a public repo as per the image: 

![Repo-Setup)](https://user-images.githubusercontent.com/77791957/116328598-6026fc00-a797-11eb-8952-651133884c02.png)

-Configured the workflow as per the image:

![Workflow](https://user-images.githubusercontent.com/77791957/116328543-3ff73d00-a797-11eb-82e0-d3363baf0c6c.png)

I did have trouble at first but that was because I forgot that i had the build-push-action@v2 rather than v1

-Then I pulled the repo from Dockerhub and made sure it was working:

![Working Dockerhub](https://user-images.githubusercontent.com/77791957/116328617-6917cd80-a797-11eb-92f9-3803bd18b54d.png)
