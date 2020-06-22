FROM openjdk:8-jdk-alpine
RUN addgroup -S spring && adduser -S spring -G spring
USER spring:spring
cp /home/edureka/jenkins/workspace/edureka-devops-automation-test/gs-spring-boot/complete/target/spring-boot-0.0.1-SNAPSHOT.jar app.jar
ENTRYPOINT ["java","-jar","-Dserver.port=8081",/app.jar"]