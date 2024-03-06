FROM gradle:8.6.0-jdk11

WORKDIR /app

COPY . .

RUN ./gradlew clean build && ls -la build/libs/

EXPOSE 8080

ENV POSTGRES_USER=kodilla
ENV POSTGRES_PASSWORD=kodilla
ENV POSTGRES_DB=kodilla-quotes 

CMD ["java", "-jar", "build/libs/quotes-0.0.1-SNAPSHOT.jar"]
