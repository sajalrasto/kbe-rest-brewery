FROM openjdk:11-jre-slim

ENV JAVA_OPTS " -Xms512m -Xmx512m -Djava.security.egd=file:/dev/./urandom"

WORKDIR application

COPY /home/ec2-user/jenkins/workspace/brew-project/target/kbe-rest-brewery-0.0.1-SNAPSHOT.war ./

ENTRYPOINT ["java", "-jar", "kbe-rest-brewery-0.0.1-SNAPSHOT.war"]
