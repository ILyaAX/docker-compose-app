FROM alpine:3.16
WORKDIR /opt
RUN apk update && apk add openjdk8-jre-base
RUN wget https://archive.apache.org/dist/tomcat/tomcat-6/v6.0.0/bin/apache-tomcat-6.0.0.tar.gz && \
	tar -xvzf apache-tomcat-6.0.0.tar.gz && \
	rm apache-tomcat-6.0.0.tar.gz
EXPOSE 8080
CMD ["/opt/apache-tomcat-6.0.0/bin/catalina.sh", "run"]