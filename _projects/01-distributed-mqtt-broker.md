---
layout: page
title: Distributed MQTT Broker
description: load-balanced, Redis-synchronised MQTT broker cluster for large-scale IoT · IEEE ESCI 2024
img: assets/img/mqtt-broker.png
importance: 1
category: distributed systems
---

Final-year project at PICT with Rohan Doshi and Tanmay Karmarkar, sponsored and mentored by Ishan Daga from Golain and guided by Prof. Madhuri Wakode.

Traditional MQTT brokers run as a single node, which works for small and medium IoT deployments but limits scale, redundancy and fault tolerance. We designed a distributed broker cluster:

- a **load balancer** forwards incoming TCP packets across broker nodes so each node is used equally;
- **Redis** is the synchronisation layer, holding shared state so any broker can serve any client;
- broker nodes form a cluster that can grow horizontally.

The work was published at the **2024 International Conference on Emerging Smart Computing and Informatics (IEEE ESCI 2024)**, Pune: <a href="https://ieeexplore.ieee.org/document/10497427">IEEE Xplore</a> (DOI: 10.1109/ESCI59607.2024.10497427). It also won **2nd Runner-Up** in the Concepts (CN domain) track at INC 2024 — Impetus and Concepts, PICT.
