DEMO - SPRING BOOT MVC, THYMELEAF AND DOCKER
============================================


LOCALHOST URL
-------------

* **URL**: http://localhost:8080


DESCRIPTION
-----------

This is simple Spring Boot MVC project which displays "Hello World" text. 

Used technologies:
* **BE**: Spring Boot MVC
* **FE**: Thymeleaf


IMPLEMENTATION
-----------

Implementation details:
* Create file pom.xml with all necessary Spring Boot dependencies;
* Create Application class with name Application to run project;
* Create Controller class with name GreetingController;
* Create Command class with name GreetingCommand;
* Create HTML template with name "greeting.html";
* Create file with CSS: src/main/resources/static/css/custom.css;
* Create file with JS: src/main/resources/static/js/custom.js.
  

LAUNCH
------

To launch project please run following class: 
* Application.java

You can also launch project using Maven command:
* mvn spring-boot:run -Dspring.thymeleaf.cache=false


USAGE
-----

Link to main UI:
* http://[server]


DOCKER
-----

Docker configuration is described in file **Dockerfile**. 
Commands:
* **Build Docker Image** (pay attention on the dot at the end): docker build -t {image-name} .
* **Run Docker Container**: docker run -p {port} {image-name}

For instance:
* docker build -t wisniewskikr/demo .
* docker run -p 8080:8080 wisniewskikr/demo 
