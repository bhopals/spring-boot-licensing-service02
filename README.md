# Introduction
Spring Microservices. 

This code example focuses on building a single service called the licensing service.  After you have compiled and started the code you should have a service called the licensing service up and running.

# Software needed
1.	Apache Maven (http://maven.apache.org)
2.	Docker (http://docker.com)
3.	Git Client (http://git-scm.com)

# Building the Docker Images

Run the following maven command.  This command will execute the [Spotify docker plugin](https://github.com/spotify/docker-maven-plugin) defined in the pom.xml file.  

   **mvn clean package docker:build**

If everything builds successfully you should see a message indicating that the build was successful.

# Running the services 

Now we are going to use docker-compose to start the actual image.  To start the docker image,
change to the directory containing. Issue the following docker-compose command:

   **docker-compose -f docker/common/docker-compose.yml up**

If everything starts correctly you should see a bunch of Spring Boot information fly by on standard out.