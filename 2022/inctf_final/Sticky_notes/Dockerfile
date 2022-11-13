FROM openjdk:20-ea-20-jdk-slim
RUN apt-get update && apt-get -y install netcat && apt-get clean
COPY deployment /usr/src/sticky_notes
WORKDIR /usr/src/sticky_notes
CMD ["java", "-jar","Sticky_notes.jar"]