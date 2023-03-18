
FROM maven:3.6.1-jdk-8-alpine AS maven_builder
WORKDIR /app
COPY pom.xml /app/pom.xml
RUN mvn dependency:go-offline -B
RUN mvn clean install
ADD . /app

FROM tomcat:8.5.43-jdk8
RUN rm -rf  /usr/local/tomcat/webapps/ROO* /usr/local/tomcat/conf/tomcat-users.xml 
COPY --from=maven_builder /app/sample.war /usr/local/tomcat/webapps/ROOT.war
# COPY --from=maven_builder /app/tomcat-users.xml /usr/local/tomcat/conf/tomcat-users.xml 
EXPOSE 8080
CMD ["/usr/local/tomcat/bin/catalina.sh", "run"]