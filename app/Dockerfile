FROM tomcat:9.0.20-jre8-alpine
WORKDIR /usr/local/tomcat
ADD config ROOT/Config.properties
RUN rm -rf /usr/local/tomcat/webapps/*
ENV WAR_FILE_PATH=${WAR_FILE_PATH}
CMD mv $WAR_FILE_PATH /usr/local/tomcat/webapps/ROOT.war \
    && catalina.sh run
