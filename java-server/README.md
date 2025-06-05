# Library App, Java version

This folder contains the Java implementation of the Library app. Is a Java Spring Boot API that exposes some routes on port 5000 by default. This app has been built to maintain as much compatibility as possible with the original Node Express server (you can have a look at that implementation in `/server`). The goal was to use the same client app for both server implementations. 
This version follows a modular hexagonal architecture, and the code is organized into three main modules:

- domain: core business logic and domain entities
- application: use cases and application services
- infrastructure: infrastructure concerns like database access and external APIs- 

# How to Build
From the project root, run:

````
mvn clean install
````

# How to Run
Make sure to set your DATABASE_URI and then start the app:

````
export MONGODB_URI=<YOUR_CONNECTION_STRING> mvn spring-boot:run
````