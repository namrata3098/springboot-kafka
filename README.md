This is a demo project using spring boot and kafka on local host to be able to produce and consume messages real time on windows machine. 
Pre-requites to run this: Apache kafka installed, Java 17, Postman and Spring bundle( dependency: web services, kafka)
To start the working:
- Run the KAFKA ZOOKEEPER using:.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties
- Run the KAFKA server using: .\bin\windows\kafka-server-start.bat .\config\server.properties
- Clone this repository and run KafkaTutorialApplication class.
- Use postman and hit the end points: http://localhost:8080/api/v1/kafka/publishjson with a JSON body according to the User class in the application.(JSONDeserialiser, JSONSerializer)
- Use postman to  hit the end points: http://localhost:8080/api/v1/kafka/publish?message=hello world without any body to use string messages.(Deserialiser, Serializer)
- Terminal will show you the messages processed.
