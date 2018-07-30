# simple-rest-service

This is a simple rest service running in spring boot deployed in a docker container

In a terminal window, clone the repo:

> git clone https://github.com/fletcher86/simple-rest-service.git

> cd simple-rest-service

Build the service in a spring boot docker container
> ./gradlew clean build docker

Run the service in a docker container for isolation
> docker run -p 8080:8080 -t fletcher68/simple-rest-service

Or Run the service in your local environment without docker
> java -jar ./build/libs/simple-rest-service-0.1.0.jar

In another terminal window, test the rest service

> curl localhost:8080

Produces the following output:

<pre>
Greetings from Spring Boot!
</pre>
