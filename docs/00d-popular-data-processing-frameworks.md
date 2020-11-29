# Different distributed systems available

As of today(28-Nov-2020), There are multiple distributed data processing system.

**Popular one are** :

- Apache Hadoop
- Apache flint
- Apache Spark
- Apache Storm
- Apache kafka & many more.

## Evolution of distributed data processing system

- 2004 | MapReduce paper was release by Google | Apache Hadoop >> two step processing one is MAP and REDUCE.
- In between apache and google worked on many product. Google products were internal, however we below describe the products of Apache.
- 2014 spark came into play and promised 100 time faster than hadoop.
- 2016 Flint came after spark with limitation of spark and considered data stream as first class citizen.
- Beam was release by Apache on june 2016, google was the major contributor.

## Apache Hadoop (MapReduce | batch | disk operation)

MapReduce is a programming model written for managing distributed data processing across several different machines in a cluster, distributing tasks to several machines, running work in parallel, managing all the communication and data transfer within different parts of the system.

The Map part of the programming model involves sorting the data based on a parameter and the Reduce part involves summarizing the sorted data.

The most popular open source implementation of the MapReduce programming model is Apache Hadoop.

The framework is used by all big guns in the industry to manage massive amounts of data in their system. It is used by Twitter for analytics. It is used by Facebook storing big data.

In real world multiple map phases are required and with multiple HDFS read and write Hadoop soon shown flaws for many business cases.

## Apache Spark

Apache Spark is an open-source cluster computing framework. It provides high performance for both batch & real-time in-stream processing.

It can work with diverse data sources & facilitates parallel execution of work in a cluster.

Spark has a cluster manager and distributed data storage. The cluster manager facilitates communication between different nodes running together in a cluster whereas the distributed storage facilitates storage of big data.

Spark seamlessly integrates with distributed data stores like Cassandra, HDFS, MapReduce File System, Amazon S3 etc.

RDD(resilient distributed dataset) are for batch processing and data stream for stream processing.

Spark do not have any mechanism to manage the late data or out of order element, Windowing watermarking was not possible.

## Apache Storm

Apache Storm is a distributed stream processing framework. In the industry, it is primarily used for processing massive amounts of streaming data.

It has several different use cases such as real-time analytics, machine learning, distributed remote procedure calls etc.

## Apache Kafka

Apache Kafka is an open-source distributed stream processing & messaging platform. It’s written using Java & Scala & was developed by LinkedIn.

The storage layer of Kafka involves a distributed scalable pub/sub message queue. It helps read & write streams of data like a messaging system.

Kafka is used in the industry to develop real-time features such as notification platforms, managing streams of massive amounts of data, monitoring website activity & metrics, messaging, log aggregation.

Hadoop is preferred for batch processing of data whereas Spark, Kafka & Storm are preferred for processing real-time streaming data.

Live example of about kafka using nodeJS: https://github.com/iAbhishek91/kafka-helm