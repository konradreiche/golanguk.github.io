---
title: "Building your own log-based message queue in Go"
metatitle: "Log-based message queue in Go"
speaker: Víctor Ruiz
video-id: ysjcEN548yc
length: "0:24:14"
---
As applications become more data-intensive and with the rise of event based architectures, terms like stream processing, ETL and data integration, become normal vocabulary for many organizations. At the center of many of these systems we find Apache Kafka, the state of the art when it comes to storing and moving around large amounts of data.<br><br>Kafka, together with Zookeeper, forms a large and complex system. But some of its unique properties like strong ordering and constant time read/write derive from its simple core data structure, the log. We'll briefly define what’s really a “log”, and how logs are at the core of many data stores.<br><br>We’ll see how a fully functional log-based queue can be rather simple to implement, you can build it yourself, and in this talk I’ll show how I’ve been building my own.<br><br>We’ll walk through the basic building blocks required to implement a pub/sub queue around a log. Segments, data indexes, offset management, etc. While I demo NetLog (netlog.io), my attempt to create a lightweight and easy-to-use log-based message queue in Go. And BigLog, its building blocks library that you can use to create your own queue.