# simple-rest-service

This is a simple rest service running in a spring boot deployed in a docker container

Clone the repo:

> git clone https://github.com/fletcher86/simple-rest-service.git

> cd simple-rest-service

Build the service in a spring boot container
> ./gradlew clean build docker

Run the service in a docker container for isolation
> docker run -p 8080:8080 -t fletcher68/simple-rest-service

Run the service in your local environment
> java -jar ./build/libs

Test the rest service

> curl localhost:8080

