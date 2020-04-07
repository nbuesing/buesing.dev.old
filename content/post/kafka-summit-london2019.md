---
title: Where are my Keys?
date: 2020-01-01
excerpt: Using Location Data to Showcase Keys, Windows, and Joins in Kafka Streams DSL and KSQL
authors:
  - Neil Buesing
---

Sometimes the hard part to Kafka Streams is understanding how to partition the data.

My talk was titled "Using Location Data to Showcase Keys, Windows, and Joins in Kafka Streams DSL and KSQL",
it really should have been "Where's My Keys".

# Link

[Using Location Data to Showcase Keys, Windows, and Joins in Kafka Streams DSL and KSQL](https://www.confluent.io/kafka-summit-lon19/using-location-data-showcase-keys-windows-joins)

# Abstract

Kafka Streams and the addition of KSQL has provided opportunities do stateful processing of data. Sometimes, 
the biggest challenge is determining how you can join that data. Keying and windowing are core concepts that 
need to be understood in order to properly and efficiently stream data. In this presentation, 
Neil will utilize geospatial data to showcase non-trivial joining; particularly, but not limited to, distance comparisons. 
The stream processing will be written in Kafka Streams DSL and in KSQL with the topologies being compared. 
KSQL 2.0 concepts of User Defined Functions (UDFs), nested AVRO structures, and ‘insert into’ functionality 
of KSQL will be showcased.

The presentation will show a custom OpenSky Connector for obtaining real-time aircraft, 
a Streams application for processing that data, a D3 topojson application to visualize the data, 
and an addition KSQL implementation of the streams application for comparison. Expect a deep dive into 
the Streams DSL and KSQL implementations that will provide the bases into a discussion around Apache Kafka 
and stream processing.