FROM eclipse-temurin:17-jdk-alpine

WORKDIR /app

COPY target/config-server-*.jar config-server.jar

EXPOSE 8080

ENTRYPOINT ["java", "-jar", "config-server.jar"]