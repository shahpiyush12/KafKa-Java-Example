"# Apache-Kafka-Tutorials"

INSTALL ZOOKEEPER; Kafka

START ZOOKEEPER

C:\devtools\kafka\kafka_2.11-1.0.0\bin\windows>zookeeper-server-start.bat ../../config/zookeeper.properties

START KAFKA SERVER

C:\devtools\kafka\kafka_2.11-1.0.0\bin\windows>kafka-server-start.bat ../../config/server.properties

SET MAVEN_HOME=c:\devtools\apache-maven-3.5.0

SET JAVA_HOME=C:\Program Files\Java\jdk1.8.0_144

SET ZOOKEEPER_HOME=C:\zookeeper\zookeeper-3.4.10

SET PATH=%PATH%;c:\devtools\spring-1.4.0.BUILD-SNAPSHOT\bin;c:\devtools\apache-maven-3.5.0\bin;C:\zookeeper\zookeeper-3.4.10\bin;.

mvn clean install

mvn -Dmainclass=com.pge.kafka.ProducerTest spring-boot:run

mvn -Dmainclass=com.pge.kafka.ConsumerTest spring-boot:run