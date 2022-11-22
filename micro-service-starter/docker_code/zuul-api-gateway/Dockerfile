FROM maven:3.8.6-openjdk-11 AS build
LABEL maintainer="edmondmgodwin@outlook.com"
WORKDIR /app
COPY . .
RUN clean install

FROM openjdk:8-jre-alpine3.9
COPY --from=build /app/target/zuul-0.0.1-SNAPSHOT.jar /zuul.jar
CMD [ "java", "-jar", "zuul-o.o.1-SNAPSHOT.jar" ]