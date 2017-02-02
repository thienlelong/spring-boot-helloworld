FROM java:8

EXPOSE 8080
VOLUME /tmp
ADD spring-boot-helloworld.jar app.jar
RUN sh -c 'touch /app.jar'
ENV JAVA_OPTS=""
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom", "-jar", "/app.jar"]
