FROM centos:8
RUN mkdir /opt/tomcat/
ADD . /opt/tomcat
WORKDIR /opt/tomcat
RUN ls -A
RUN tar xvfz apache*.tar.gz
RUN mv /opt/tomcat/apache-tomcat-8.5.85/* /opt/tomcat
RUN ls -A
RUN rpm -ivh jdk-8u361-linux-x64.rpm 
RUN java -version
RUN rm -rf /opt/tomcat/jdk-8u361-linux-x64.rpm /opt/tomcat/webapps/* /opt/tomcat/Dockerfil* /opt/tomcat/apache*
RUN mv sample.war /opt/tomcat/webapps/ROOT.war
WORKDIR /opt/tomcat/webapps
RUN ls -A
EXPOSE 8080
CMD ["/opt/tomcat/bin/catalina.sh", "run"]