getting-start-with-spring-data-rest
============

A Basic Spring Data JPA app with an H2 DB running on Spring Boot

Prerequisites
-------------
You will need to following tools in order to work with this project and code

* git (http://git-scm.com/)
* JDK 1.8+ (http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
* Maven 3.x+ (http://maven.apache.org/)
* Gradle 2.8
* An IDE of your choice.  (Eclipse, IntelliJ, Spring STS, Netbeans, etc.)

Getting Started
---------------
To run this project locally, perform the following steps.

* Clone project to your machine using git - "git clone https://github.com/dlbunker/ps-guitar-rest.git"
* Import the project into your IDE using the maven pom.xml.  In spring STS suite this is done by importing
an existing maven project
* Next try running the app as a Spring Boot app.  You can do this by running the Main.java file in this
project as a standard java project or you can run spring boot at your project's root with Maven using the
following command.  'mvn spring-boot:run'
* Or from gradle : 
$ gradle build
$ java -jar build/libs/getting-start-spring-data-rest-0.1.0.jar

To test the REST services are loaded:
- go to a browser ( like Chrome ) : chrome://apps/
- install Postman which is used to send request for Service Level 3 ( with Request verbs )
- send :
   - GET
   - on with URL : http://localhost:8080/api
   - having on HEADERS :
         - Content-Type : application/json
         - And add Authorization with Basic Auth and pass admin / admin for username / password
		 (should be something like -> Authorization : Basic YWRtaW46YWRtaW4=)
