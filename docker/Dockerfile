ARG CORA_DOCKER_JAVA_VERSION
FROM cora-docker-java:${CORA_DOCKER_JAVA_VERSION}

COPY /divaindexmessenger*.jar /indexing/divaindexmessenger.jar

COPY /*.properties /indexing/properties/

WORKDIR /indexing

CMD java -classpath /indexing/properties/:/indexing/divaindexmessenger.jar \
se.uu.ub.cora.diva.indexmessenger.DivaIndexMessengerStarter \
${hostname} ${port} ${routingKey} ${username} ${password} \
${appTokenVerifierUrl} ${baseUrl} ${userId} ${appToken} 