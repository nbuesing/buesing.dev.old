---
title: Building an Enterprise Eventing Framework
date: 2020-02-01
excerpt: Bryan Zelle presents on the work done at Centene; I present a visual demo of the application.
authors:
  - Neil Buesing
---

How Centene built an eventing framework available within 6 months of starting development.

# Link

[Building an Enterprise Eventing Framework](https://www.confluent.io/kafka-summit-san-francisco-2019/building-an-enterprise-eventing-framework)

# Abstract

Centene is fundamentally modernizing its legacy monolithic systems to support distributed, real-time event-driven healthcare 
information processing. A key part of our architecture is the development of a universal eventing framework to accommodate 
transformation into an event-driven architecture (EDA). Our application provides a representational state transfer (REST) 
and remote procedure call (gRPC) interface that allows development teams to publish and consume events with a simple 
Noun-Verb-Object (NVO) syntax. Embedded within the framework are structured schema evolutions with Confluent Schema Registry 
and AVRO, configurable (self-service) event-routing with K-Tables, dynamic event-aggregation with Kafka Streams, distributed 
event-tracing with Jaeger, and event querying against a MongoDB event-store hydrated by Kafka Connect. Lastly, we developed 
techniques to handle long-term event storage within Kafka; specifically surrounding the automated deletion of expired events 
and re-hydration of missing events. In Centene's first business use case, events related to claim processing of provider 
reconsiderations was used to provide real-time updates to providers on the status of their claim appeals. To satisfy the 
business requirement, multiple monolith systems independently leveraged the event framework, to stream status updates for 
display on the Centene Provider Portal instantly. This provided a capability that was brand new to Centene: the ability to 
interact and engage with our providers in real-time through the use of event streams. In this presentation, we will walk 
you through the architecture of the eventing framework and showcase how our business requirements within our claims adjudication 
domain were able to be solved leveraging the Kafka Stream DSL and the Confluent Platform. And more importantly, how Centene 
plans on leveraging this framework, written on-top of Kafka Streams, to change our culture from batch processing to real-time 
stream processing.