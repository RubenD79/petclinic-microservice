FROM openjdk:11-jre



ENV SPRING_PROFILES_ACTIVE docker,mysql
ADD ./target/*.jar /app.jar
ADD https://github.com/jwilder/dockerize/releases/download/${DOCKERIZE_VERSION}/dockerize-alpine-linux-amd64-${DOCKERIZE_VERSION}.tar.gz dockerize.tar.gz



ENTRYPOINT  java -jar /app.jar 