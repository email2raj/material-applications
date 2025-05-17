# 5-17-2025
# install the java 8 from amazon docker hub - The project should open in 8080 and you get a message by pressing the button.

FROM amazoncorretto:8

#expose the port your app runs on
EXPOSE 8080

#Set the working dir inside the container
WORKDIR /usr/src/app

#Build the project with ./mvnw package
RUN ./mvnw package

#Run with java -jar ./target/docker-example-1.1.3.jar
CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]

