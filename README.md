## Project Name
Dockerize a tomcat Application

## Author
 - Name : Eliud Gateri
 - Email: egateri@gmail.com

## About this project
How to dockerize a tomcat application

## Instructions to use this project
1. Creat a project folder
1. Download apache-tomcat-8.5.85.tar.gz and jdk-8u361-linux-x64.rpm onto the project folder
1. git clone https://github.com/egateri/tomcat.git   --> to get the Dockerfile and sample.war files
1. You may replace sample.war with your working WAR file
1. Ensure docker is up and running
1. docker build -t tomcat-app .
1. docker run -d -p 8080:8080 tomcat-app
1. Access your servlets via http://localhost:8080

## Live link


## Technologies and Languages used
 * Technologies
 1. Docker

## License
(c) 2023 Eliud Gateri

