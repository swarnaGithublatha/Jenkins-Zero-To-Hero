# You can change this base image to anything else
# But make sure to use the correct version of Java
# FROM adoptopenjdk/openjdk11:alpine-jre

# # Simply the artifact path
# ARG artifact=target/spring-boot-web.jar

# WORKDIR /opt/app

# COPY ${artifact} app.jar

# # This should not be changed
# ENTRYPOINT ["java","-jar","app.jar"]
# Use a base image with the Java runtime environment
FROM adoptopenjdk/openjdk11:alpine-jre

# Set the working directory inside the container
WORKDIR /app

# Copy the compiled Java application JAR file into the container
COPY target/my-java-app.jar /app/my-java-app.jar

# Define the command to run the Java application when the container starts
CMD ["java", "-jar", "my-java-app.jar"]
