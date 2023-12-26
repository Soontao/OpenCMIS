# Use the official Tomcat 9 image as the base image
FROM maven:eclipse-temurin-21 AS builder

WORKDIR /build

COPY . .

RUN mvn clean package

FROM tomcat:9-jdk21

# Set the working directory to the Tomcat webapps directory
WORKDIR /usr/local/tomcat/webapps/

# Remove the default ROOT application
RUN rm -rf ROOT

# Copy your WAR file into the webapps directory
COPY --from=builder /build/chemistry-opencmis-server/chemistry-opencmis-server-inmemory/target/chemistry-opencmis-server-inmemory-*-SNAPSHOT.war ROOT.war

# Expose the default Tomcat port
EXPOSE 8080

# Start Tomcat when the container starts
CMD ["catalina.sh", "run"]
