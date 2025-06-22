FROM eclipse-temurin:17-jdk-alpine

WORKDIR /app

COPY target/musics-service-*.jar musics-service.jar

EXPOSE 8080

ENTRYPOINT ["java", "-jar", "musics-service.jar"]