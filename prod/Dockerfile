FROM alpine:3.16
WORKDIR /opt
RUN apk update && apk add openjdk7-jre-base
RUN wget https://archive.apache.org/dist/tomcat/tomcat-6/v6.0.16/bin/apache-tomcat-6.0.16.tar.gz && \
	tar -xvzf apache-tomcat-6.0.16.tar.gz && \
	rm apache-tomcat-6.0.16.tar.gz
EXPOSE 8080
CMD ["/opt/apache-tomcat-6.0.16/bin/catalina.sh", "run"]