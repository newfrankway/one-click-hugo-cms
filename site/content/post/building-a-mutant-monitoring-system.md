---
title: Building a Mutant Monitoring System
date: 2023-04-01T14:45:48.295Z
description: >-
  Overview


  This course touches on different topics, providing a backstory that is relevant for the first few lessons. The lessons can be taken independently of one another. Some of the topics covered in the course are covered more in-depth in other courses. In such cases, a link is provided to other lessons and material.
---
### Backstory

Mutants have emerged from the shadows and are wreaking havoc on the earth! Increased levels of malicious mutant behavior pose a threat to national security and the general public. Luckily, some mutants have teamed up with Government agencies to help protect people against the bad ones.

To better protect the citizens and understand more about the mutants, the Government enacted the Mutant Registration Act. As required by the act, each mutant must wear a small device that reports on their actions every second.

Your mission, as a new member of Division 3, is to help the Government keep the Mutants under control by building a Mutant Monitoring System (MMS). The MMS will consist of a database that will contain a Mutant Catalog and Monitoring system.

### Choosing a Database

A NoSQL database is preferred for MMS because it has high availability, a scale-out data set, disaster recovery capabilities, and can accommodate IoT time-series workloads – all the requirements for the MMS database. There are many NoSQL database technologies to choose from, such as HBase, Apache Cassandra, MongoDB, Influx, and ScyllaDB.

ScyllaDB was chosen for the MMS because it leverages the best from Apache Cassandra in high availability, fault tolerance, and rich ecosystem. ScyllaDB provides a dramatically higher-performing and resource-effective NoSQL database to power modern and demanding applications with low latencies and none of the Java garbage collection woes found in other NoSQL databases.

A collection of data on each mutant needs to be imported into the database. The Mutant Catalog database will keep track of basic contact information for each mutant, including the mutant’s first name, last name, address, and photo.

To monitor the mutants, we need a separate tracking database consisting of time-series data such as the mutant’s location, speed, velocity, heat, and telepathy powers. The data will be gathered from various sources and imported into the database. After the data is gathered, we will be able to analyze the statistics.

### Setting up a Cluster

Before we proceed, follow [this](https://university.scylladb.com/setup-a-scylla-cluster/) procedure to set up a ScyllaDB cluster.