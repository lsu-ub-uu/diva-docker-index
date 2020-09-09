FROM  openjdk:14

COPY /divaindexmessenger*.jar /indexing/divaindexmessenger.jar
#COPY /activemq.jar /indexing/activemq.jar
#COPY /log4j.jar /indexing/log4j.jar

COPY /*.properties /indexing/properties/

WORKDIR /indexing

#CMD java -classpath /indexing/properties/:/indexing/activemq.jar:/indexing/divaindexmessenger.jar:/indexing/log4j.jar se.uu.ub.cora.diva.indexmessenger.DivaIndexMessengerStarter

CMD java -classpath /indexing/properties/:/indexing/divaindexmessenger.jar se.uu.ub.cora.diva.indexmessenger.DivaIndexMessengerStarter