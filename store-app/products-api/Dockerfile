FROM gradle:8.6.0-jdk11

WORKDIR /app

COPY . .

RUN ./gradlew clean build && ls -la build/libs/

EXPOSE 8080

CMD ["java", "-jar", "build/libs/products-api-0.0.1-SNAPSHOT.jar"]