FROM maven:3.8.6-openjdk-11 AS build
LABEL maintainer="edmondmgodwin@outlook.com"
WORKDIR /app
COPY . .
RUN mvn clean install

FROM openjdk:11.0.14-jre
COPY --from=build /app/target/zuul-0.0.1-SNAPSHOT.jar /zuul.jar
CMD [ "java", "-jar", "zuul.jar" ]