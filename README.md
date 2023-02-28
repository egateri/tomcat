### Project Name
Dockerize a tomcat Application

### Author
 - Name : Eliud Gateri
 - Email: egateri@gmail.com

### About this project
How to dockerize a tomcat application

### Instructions to use this project
 Creat a project folder   
 Download _apache-tomcat-8.5.85.tar.gz_ and _jdk-8u361-linux-x64.rpm_ onto the project folder  
 To get the _Dockerfile_ and _sample.war_ files  
 `git clone https://github.com/egateri/tomcat.git`   
 You may replace sample.war with your working WAR file  
 Ensure docker is up and running  
 Run below command to build the image  
  `docker build -t tomcat-app .`  
 Run below command to run the container in docker  
  `docker run -d -p 8080:8080 tomcat-app`  
 Access your servlets via **http://localhost:8080**  

### Technologies and Languages used
 * Technologies
 1. Docker

### License
(c) 2023 Eliud Gateri

