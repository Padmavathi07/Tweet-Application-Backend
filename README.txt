/* To Start and run the Application Please follow the below Steps */

Step-1 : Start the Zookeeper using the below command in cmd

$ C:\kafka_2.12-2.8.1\bin\windows\zookeeper-server-start.bat C:\kafka_2.12-2.8.1\config\zookeeper.properties

Step-2 : Start the Kafka Server using the below command in cmd

$ C:\kafka_2.12-2.8.1\bin\windows\kafka-server-start.bat C:\kafka_2.12-2.8.1\config\server.properties

******************Step-3 : Execute the below command in cmd for the first time only.....****************************************
To Create the kafka topic for the first time use belwo cmd

$ C:\kafka_2.12-2.8.1\bin\windows\kafka-topics.bat -zookeeper localhost:2181 -topic kafkaMessage --create --partitions 3 --replication-factor 1


To List the Kafka Topics  go to C:\kafka_2.12-2.8.1\bin\windows\ and use below cmd

$ kafka-topics.bat --list --zookeeper localhost:2181

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Step-4 : Start the Application in STS/Eclipse 

Step-5 : Check whether the actuator is working or not using the below link in Web-browser.(usage: to check the Health of the apllication)

localhost:8090/actuator


Step-6 : Go to Prometheus folder and open cmd for that path...and then execute this command(usage: to check the Performance the Application in UI graph) 

$ prometheus


Step-7 : Check whether the prometheus is working or not using the below link in Web-browser

http://localhost:9090


Step-8 : Go to Grafan Bin folder and open cmd for this path.....and then execute this command (uasgae: to check the Performance the Application in UI graph)

$ grafana-server

http://localhost:3000

cred's: admin/admin	


Step-9 : Go to Elasticsearch  Bin folder and open cmd for this path....and thenn execute this command

$ elasticsearch


Step-10 : Go to Logstash Bin folder and open cmd for this path....and thenn execute this command 

before that place the logstash.conf file into bin folder by specifing the tweetlog.log file path in logstash.conf


logstash -f logstash.conf


Step-11 : Check whether the Logstash is working or not using the below link in Web-browser

http://localhost:9200/_cat/indices


Step-12 : Go to Kibana Bin folder and open cmd for this path....and then execute this command

$ kibana

Step-13 : Check whether the Kibana is working or not using the below link in Web-browser

http://localhost:5601

Step-14:

API Calls for the Tweet App (Swagger UI)

http://localhost:8090/swagger-ui.html#/


