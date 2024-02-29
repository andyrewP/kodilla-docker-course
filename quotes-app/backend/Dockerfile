FROM ubuntu

WORKDIR /app

COPY . .

RUN apt-get update && \
    apt-get install -y openjdk-11-jdk;

RUN ./gradlew clean build && ls -la build/libs/

EXPOSE 8080

CMD ["java", "-jar", "build/libs/quotes-0.0.1-SNAPSHOT.jar"]