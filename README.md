# Getting Started with Confluent

To get started with Confluent, follow these steps:

1. **Install the Confluent CLI.**

2. **Start the Kafka broker** by running the following command: `confluent local kafka start`
After starting the Kafka broker, note the Plaintext Ports printed in your output terminal. Copy this value and paste it in the `kafka-configurations.properties` file.

3. **Create a new topic.** For example, to create a topic called `purchases`, run the following command: `confluent local kafka topic create purchases`

4. **Run a producer** to produce events to the `purchases` topic. Use the following command: `./out/producer kafka-configurations.properties`
The output will show all ten events created.

5. **To consume these events**, run the following command: `./out/consumer kafka-configurations.properties`
After consuming the events, press `CTRL + C` to terminate the application.

This is a basic guide to getting started with Confluent. For more advanced usage, refer to the Confluent documentation.
