#### Project Name
Dockerize a tomcat Application
#### Author
 - Name : Eliud Gateri
 - Email: egateri@gmail.com
#### About this project
How to dockerize a tomcat application
#### Instructions to use this project  
1. Create a project folder from command line.      
    
    `$mkdir your_project_folder`   
    
2. Navigate to to your project folder.      
   
    `$cd your_project_folder`

2.  Clone the _tomcat_ project into your project folder above.    
        
    `$git clone https://github.com/egateri/tomcat.git`    

 3. You should have two subfolders *option_1* and *option_2* within _tomcat_   
          
   

 ##### OPTION 1   - Download required and takes more time
 1. Navigate to the *option_1* subfolder.  
    
    `$cd tomcat/option_1`    
       
 2. Download _apache-tomcat-8.5.85.tar.gz_ and _jdk-8u361-linux-x64.rpm_ and save the files inside *your_project_folder/tomcat/option_1*   

 3. You may replace _sample.war_ with your working WAR file inside *option_1*  
   folder    
   **NOTE:** Save your WAR file as _sample.war_ or edit the _Dockerfile_ to capture the correct name of your WAR file.   
      
5. Ensure docker is up and running.  
      
   `$docker version` 
     
5. Run below command to build the image.   
     
   `$docker build -t tomcat-app1 .`   
       
6. Run below command to run the container in docker.   
       
   `$docker run -d -p 8081:8080 tomcat-app1`   
      
7. Confirm if the container is running.    
       
   `$docker ps -a`   
     
8. Access your dockerized tomcat application via *http://localhost:8081* on    
    the  broswer or  `$curl http://localhost:8081` from command line   
      

 ##### OPTION 2 (POM.XML - No download require & Faster)    

       
           
    
  1. Navigate to the *option_2* subfolder.   
    `$cd tomcat/option_2`    
  2. You may replace _sample.war_ with your working WAR file inside *option_2* folder
   **NOTE:** Save your WAR file as _sample.war_ or edit the _Dockerfile_ to capture the correct name of your WAR file.  
        
  3. Ensure docker is up and running.  
      
      `$docker version` 
     
5. Run below command to build the image.     
       
    `$docker build -t tomcat-app2 .`   
         
6. Run below command to run the container in docker.   
       
    `$docker run -d -p 8082:8080 tomcat-app2`   
      
7. Confirm if the container is running.    
       
    `$docker ps -a`   
     
8. Access your dockerized tomcat application via *http://localhost:8082* on the  
   broswer or   `$curl http://localhost:8082` from command line.   
 
#### Technologies and Languages used
 1. Docker
####  License
(c) 2023 Eliud Gateri

