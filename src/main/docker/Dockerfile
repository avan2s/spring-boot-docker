FROM openjdk

VOLUME /tmp
ADD maven/${docker.fileName} ${docker.fileName}
RUN sh -c 'touch /myapp.jar'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/${docker.fileName}"]