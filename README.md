#### Project Name
Dockerize a tomcat Application
#### Author
 - Name : Eliud Gateri
 - Email: egateri@gmail.com
#### About this project
How to dockerize a tomcat application
#### Instructions to use this project
1. Creat a project folder   
2. Download _apache-tomcat-8.5.85.tar.gz_ and _jdk-8u361-linux-x64.rpm_ onto the project folder  
3. To get the _Dockerfile_ and _sample.war_ files run below command  
 `git clone https://github.com/egateri/tomcat.git`   
4. You may replace _sample.war_ with your working WAR file  
5. Ensure docker is up and running  
6. Run below command to build the image  
  `docker build -t tomcat-app .`  
 7. Run below command to run the container in docker  
  `docker run -d -p 8080:8080 tomcat-app`  
 8. Access your servlets via *http://localhost:8080*  

#### Technologies and Languages used
 1. Docker
####  License
(c) 2023 Eliud Gateri

