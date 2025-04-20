# Use a minimal JDK base image
FROM eclipse-temurin:11-jre-alpine

# Add a volume for temporary files
VOLUME /tmp

# Copy the fat JAR built by Maven
COPY target/*.jar app.jar

# Expose the application port
EXPOSE 8080

# Run the application
ENTRYPOINT ["java","-jar","/app.jar"]
