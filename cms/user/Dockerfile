FROM openjdk:11-jre-slim
COPY build/libs/user-0.0.1-SNAPSHOT.jar user.jar
ENTRYPOINT ["java","-DSpring.profiles.active=prod","-Dmailgun.key=${MAILGUN_KEY}","-jar","user.jar"]