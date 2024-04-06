# Show how to getting firsts steps in confluent
To run first install cofluent CLI, after this start kafka broken using -> confluent local kafka start
After started kafka broken in your output terminal is printed Plaintext Ports, copy this value and paste in kafka-configurations.properties.
Now you need create a new topic, lets create a topic called purchases -> confluent local kafka topic create purchases.
In the end, we need to run a producer using -> ./out/producer kafka-configurations.properties, output is show all the ten events created
For consume this events we need run -> ./out/consumer kafka-configurations.properties, after the consumed events enter CTRL + C to terminate application.

