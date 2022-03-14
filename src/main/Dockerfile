FROM java:8
VOLUME /tmp
ADD cloud_backend-1.0-SNAPSHOT.jar app.jar
RUN bash -c 'touch /root/app.jar'
EXPOSE 8761
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/root/app.jar"]
