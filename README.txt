Project structure

  / ==> project folder
  
  /                 /media
  |---------------- |
  |                 |------cat.jpeg
  |-- index.html    |   
  |                 |          /media/person  
  |                 |----------|
  |                            |--> person.png
  |                            |
  |                 /js
  |                 |
  |-----------------|
  |                 |--- index.js
  |                 |              /js/main
  |                 |--------------|
  |                                |---- main.js
  |                                |
  |                                |        /js/main/custom
  |                                |--------|
  |                                |        |
  |                                         | ----others.js
  |
  |
  |                                       /app
  |                                       |
  |                                       |
  |-------------------------------------- |--- properties.config
  |                                       |
  |                                       |------- pom.xml
  |                                       |
  |                                       |------- sample.war
  |                                      
  |
  |
  |
  |       /public
  |--------|
  |        |-----index.html
  |        |
  |        |       /html
  |        |--------| 
  |        |        |-----index.html
  |
  |
  |
  |------------ Dockerfile
  |
  | 
  |------------ docker-compose.yml
  |
  |
  |
  |                 /css
  |                 |
  |-----------------|
  |                 |-- main.css
  |                 |              /css/styles
  |                 |--------------|
  |                                |---- darkmode.css
  |                                |
  |                                |----- clearmode.css
  |                                |
  |                                |      /css/styles/customization
  |                                |--------|
  |                                |        |
  |                                         | ----custom.css