# kafka-location-update-producer
This is a demo project to implement kafka for practice where each live location (dummy data) update will be given to the end user.

required Commands
start kafka
.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties

.\bin\windows\kafka-server-start.bat .\config\server.properties

.\bin\windows\kafka-topics.bat --create --bootstrap-server localhost:9092 --topic test

.\bin\windows\kafka-console-producer.bat --broker-list localhost:9092 --topic test


.\bin\windows\kafka-console-consumer.bat --topic test --bootstrap-server localhost:9092 --from-beginning

// to stop the kafka

.\bin\windows\zookeeper-server-stop.bat .\config\zookeeper.properties

.\bin\windows\kafka-server-stop.bat .\config\server.properties
