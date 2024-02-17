# You can change this base image to anything else
# But make sure to use the correct version of Java
# FROM adoptopenjdk/openjdk11:alpine-jre

# # Simply the artifact path
# ARG artifact=target/spring-boot-web.jar

# WORKDIR /opt/app

# COPY ${artifact} app.jar

# # This should not be changed
# ENTRYPOINT ["java","-jar","app.jar"]

# Use the arm64v8/openjdk:11-jre-slim base image
FROM arm64v8/openjdk:11-jre-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the Java application JAR file into the container
COPY target/spring-boot-web.jar app.jar

# Define the command to run the Java application
CMD ["java", "-jar", "app.jar"]
