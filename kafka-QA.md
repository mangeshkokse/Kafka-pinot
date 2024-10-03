# Streaming Data from Kafka to Apache Pinot
https://medium.com/swlh/apache-kafka-what-is-and-how-it-works-e176ab31fcd5

# Q.What is Apache Kafka?
Kafka is a powerful tool used to send and receive data between different applications in real time. Think of it as a high-speed messaging system that can handle a large amount of data, allowing different systems to communicate with each other. It’s often used for streaming events, like logs, user activity, or data from sensors, making sure everything stays in sync as things happen.

- ***A distributed streaming platform*** - What is an “A distributed streaming platform”? First, we need to define what is a stream. For that, I have a definition that made me really understand it: Streams are just infinite data, data that never end. It just keeping arriving, and you can process it in real-time.
And distributed? Distributed means that Kafka works in a cluster, each node in the cluster is called Broker. Those brokers are just servers executing a copy of apache Kafka.
So, basically, Kafka is a set of machines working together to be able to handle and process real-time infinite data.
His distributed architecture is one of the reasons that made Kafka so popular. The Brokers is what makes it so resilient, reliable, scalable, and fault-tolerant. That’s why Kafka is so performer and secure.

# Q. What is Zookeeper?
Zookeeper is a coordination and synchronization service used in distributed systems. It helps manage configuration, track status, and maintain consistency across a cluster of machines or services.

### Use Case in Kafka:
In **Kafka**, Zookeeper is used to manage and coordinate the Kafka brokers (servers). It performs tasks like:
- **Leader election** for partitions, ensuring only one broker is responsible for a particular partition.
- **Configuration management**, keeping track of all brokers in the Kafka cluster.
- **State management**, maintaining metadata about topics, partitions, and replicas.
- **Failure detection**, notifying Kafka if a broker goes down, so the system can adjust.

Zookeeper helps Kafka remain reliable and consistent by ensuring that all parts of the Kafka cluster are working together in sync.

  
  
