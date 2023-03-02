#### Project Name
Dockerize a tomcat Application
#### Author
 - Name : Eliud Gateri
 - Email: egateri@gmail.com
#### About this project
How to dockerize a tomcat application
#### Instructions to use this project   
1. Run below command to get the _Dockerfile_ and _sample.war_ files cloned into a project folder.    
 `git clone https://github.com/egateri/tomcat.git`   
2. Download _apache-tomcat-8.5.85.tar.gz_ and _jdk-8u361-linux-x64.rpm_ and save the files inside the cloned project folder above 
3. You may replace _sample.war_ with your working WAR file inside the cloned project folder 
4. Ensure docker is up and running    
   `docker version` 
5. Run below command to build the image  
  `docker build -t tomcat-app .`  
6. Run below command to run the container in docker  
  `docker run -d -p 8080:8080 tomcat-app`  
7. Confirm if the container is running   
  `docker ps -a` 
8. Access your dockerized tomcat application via *http://localhost:8080*
 
#### Technologies and Languages used
 1. Docker
####  License
(c) 2023 Eliud Gateri

