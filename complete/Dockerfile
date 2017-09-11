FROM openjdk:8-jdk-alpine
VOLUME /tmp
CMD ls -al /opt/vsts/work/1/s/complete
ADD complete/build/libs/gs-spring-boot-docker-0.1.0.jar app.jar
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar" ]
