# Assuming we are running docker build from the directory of the project (which contains this Dockerfile)
# build the image with docker build . -t java-spring
FROM openjdk:8

EXPOSE 8080

WORKDIR /usr/src/app

COPY . .

# Windows users need the command below (remove spaces and CR characters - https://stackoverflow.com/questions/61226664)
RUN sed -i 's/\r$//' mvnw

RUN ./mvnw package

CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]