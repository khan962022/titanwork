FROM tomcat:8-jre11
LABEL "Author"="Khan"
LABEL "Project"="Vprofile"

WORKDIR /usr/local/tomcat
RUN rm -rf /usr/local/tomcat/webapps/*
VOLUME appdata:/usr/local/tomcat/webapps

EXPOSE 8080
COPY target/vprofile-v2.war /usr/local/tomcat/webapps/ROOT.war

CMD ["catalina.sh", "run"]
