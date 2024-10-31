FROM openjdk:8-oracle
MAINTAINER Qvbian
VOLUME /tmp
ADD docker_boot.jar /docker_boot.jar
RUN bash -c 'touch /docker_boot.jar'
ENTRYPOINT ["java","-jar","/docker_boot.jar"]
EXPOSE 6001









