FROM maven:3.8.5-openjdk-17-slim
WORKDIR /app
COPY . .
RUN chmod +x makemytour/mvnw && cd makemytour && ./mvnw clean install -DskipTests
EXPOSE 8080
ENTRYPOINT ["java", "-jar", "makemytour/target/makemytrip-0.0.1-SNAPSHOT.jar"]