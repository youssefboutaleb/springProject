# Use the official OpenJDK 17 base image
FROM openjdk:17-jdk-alpine

# Set the working directory
WORKDIR /app

# Copy the JAR file into the container
COPY target/registryService-0.0.1-SNAPSHOT.jar /app/

# Expose the port that your Spring Boot application will run on
EXPOSE 8888

# Specify the command to run your application
CMD ["java", "-jar", "registryService-0.0.1-SNAPSHOT.jar"]
