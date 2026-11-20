FROM eclipse-temurin:21

# Remove unused vulnerable Go binary inherited from the base image
RUN rm -f /usr/bin/pebble

WORKDIR /app

COPY target/gate-sonargate-demoproject-1.0.0-SNAPSHOT.jar app.jar

EXPOSE 8080

ENTRYPOINT ["java", "-jar", "app.jar"]
