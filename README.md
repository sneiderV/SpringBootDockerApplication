# Spring Boot Web Service Application & Docker 

For the person looking to create a simple web services application in sprint boot and docker; this is an easy example of what you need to know. The Dockerfile that have this project is very simple, but it is all you need to run a Spring Boot app: just Java and a JAR file.

## Technologies
- Java 1.8
- Spring boot 
- Docker

## Run on-promise
Run this snippet (_JDK 11 was used in this example to compile the application_) <br>
`mvnw package && java -jar spring-boot-docker-0.0.1-SNAPSHOT.jar`
 > You can use the following path to check the response of the app: http://localhost:8080/

## Create an image
To create an image run this command: <br>
`docker build -t spring-boot-docker . `

## Run a container
After create a spring-boot-docker image you can run a container with following command: <br>
`docker run -p 8080:8080 spring-boot-docker`
> You can use the following path to check the response of the app: http://localhost:8080/
