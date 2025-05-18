FROM amazoncorretto:8

# Set working directory
WORKDIR /usr/src/app

# Copy files needed to build the project
COPY mvnw .
COPY .mvn .mvn
COPY pom.xml .
COPY src ./src

# Make mvnw executable
RUN chmod +x ./mvnw

# Build the project using mvnw
RUN ./mvnw package

# Expose the port
EXPOSE 8080

# Run the application
CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]

