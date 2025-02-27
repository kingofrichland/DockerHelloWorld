# Use an official OpenJDK 17 runtime as the base image
FROM openjdk:17-jdk-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy the JAR file into the container
COPY target/HelloWorld-0.0.1-SNAPSHOT.jar /app/HelloWorld-0.0.1-SNAPSHOT.jar

# Expose port 8080 to the outside world
EXPOSE 8080

# Run the Spring Boot application
ENTRYPOINT ["java", "-Dspring.profiles.active=${SPRING_PROFILE}", "-jar", "HelloWorld-0.0.1-SNAPSHOT.jar"]
