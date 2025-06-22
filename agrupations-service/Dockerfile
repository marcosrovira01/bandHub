FROM eclipse-temurin:17-jdk-alpine

WORKDIR /app

COPY target/agrupations-service-*.jar agrupations-service.jar

EXPOSE 8080

ENTRYPOINT ["java", "-jar", "agrupations-service.jar"]