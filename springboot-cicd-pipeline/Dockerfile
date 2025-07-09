# My Dockerfile
# You can change this base image to anything else
# But make sure to use the correct version of Java


#Using Java 17
FROM openjdk:17-jdk-slim

#Automatically picks the jar using wildcard (*.jar)
ARG JAR_FILE=target/*.jar

#Any COPY, RUN, or CMD after that happens inside /opt/app
WORKDIR /opt/app

#...will place your JAR inside /opt/app/app.jar
COPY ${JAR_FILE} app.jar

ENTRYPOINT ["java", "-jar", "app.jar"]
