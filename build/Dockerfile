FROM maven:3.8-openjdk-8
RUN apt update
WORKDIR /opt/app
RUN git clone https://github.com/shephertz/App42PaaS-Java-MySQL-Sample.git /opt/app
COPY ./Config.properties /opt/app/WebContent/Config.properties
RUN mvn package