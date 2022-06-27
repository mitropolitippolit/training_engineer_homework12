FROM maven:3-jdk-8-alpine
ENV GIT_REPO_URL=https://github.com/shephertz/App42PaaS-Java-MySQL-Sample.git
RUN apk add --update git
WORKDIR /data
RUN git clone $GIT_REPO_URL app
WORKDIR /data/app
CMD mvn package
