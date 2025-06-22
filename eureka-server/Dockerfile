FROM eclipse-temurin:17-jdk-alpine

WORKDIR /app

COPY target/eureka-server-*.jar eureka-server.jar

EXPOSE 8080

ENTRYPOINT ["java", "-jar", "eureka-server.jar"]