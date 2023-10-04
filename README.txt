Ejecutar Zookeeper

$ C:\kafka\bin\windows\zookeeper-server-start.bat C:\kafka\config\zookeeper.properties

Ejecutar Kafka

$ C:\kafka\bin\windows\kafka-server-start.bat C:\kafka\config\server.properties

Crear topic

$ kafka-topics.bat --create --topic ######## --bootstrap-server localhost:9092

Listar topics

$ kafka-topics.bat --list --bootstrap-server localhost:9092

Crear archivo de configuraciones para el conector source

Crear archivo de configuraciones para el conector sink

Crear el archivo producer

Crear el archivo consumer

Ejecutar el pipeline


Notas:

Agregar converters al archivo de configuraciones connect-standalone.properties

 - key.converter=org.apache.kafka.connect.storage.StringConverter
 - value.converter=org.apache.kafka.connect.storage.StringConverter

Agregar el puerto para la REST API de conectores

 - rest.port=8083


