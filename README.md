"# Apache-Kafka-Tutorials"

SET MAVEN_HOME=c:\devtools\apache-maven-3.5.0

SET JAVA_HOME=C:\Program Files\Java\jdk1.8.0_144

SET ZOOKEEPER_HOME=C:\zookeeper\zookeeper-3.4.10

SET PATH=%PATH%;c:\devtools\spring-1.4.0.BUILD-SNAPSHOT\bin;c:\devtools\apache-maven-3.5.0\bin;C:\zookeeper\zookeeper-3.4.10\bin;.

mvn clean install

mvn -Dmainclass=com.pge.kafka.ProducerTest spring-boot:run
mvn -Dmainclass=com.pge.kafka.ConsumerTest spring-boot:run