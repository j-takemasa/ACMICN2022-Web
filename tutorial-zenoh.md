---
layout: default
title: "Half-day Tutorial: Zenoh: Data-Centric Communication for the Cloud-to-Things Continuum"
group: Tutorials

presenters:
- name: Angelo Corsaro
  affiliation: ZettaScale Technology
  homepage: https://www.linkedin.com/in/corsaro/
#   photo: speakers/Alex-Afanasyev.jpg
  bio: "Angelo Corsaro is the CEO/CTO at ZettaScale Technology SARL. He is a world top expert in edge/fog computing and a well-known researcher in the area of highperformance and large-scale distributed systems."

- name: Luca Cominardi
  affiliation: ZettaScale Technology
  homepage: https://www.linkedin.com/in/lucacominardi/
#   photo: speakers/Alex-Afanasyev.jpg
  bio: "Luca Cominardi received his PhD in Telematics Engineering from the University Carlos III of Madrid, Spain, in 2019. Since 2013, he has been extensively working on Edge computing and Network softwarization technologies producing in that period scientific publications, patents, open source software, and contributions to standardization in ETSI MEC. He is currently the product conductor of Zenoh."

- name: Olivier Hécart
  affiliation: ZettaScale Technology
  homepage: https://www.linkedin.com/in/olivierhecart/
#   photo: speakers/Alex-Afanasyev.jpg
  bio: "Olivier Hécart received his Engineering degree in computer science at University of Paris-Saclay in 2005. Since 2005 he acquired a great expertise in distributed systems working on CORBA and DDS technologies. Since 2018, he actively works on the design and implementation of Zenoh."

- name: Pierre Avital
  affiliation: ZettaScale Technology
  homepage: https://www.linkedin.com/in/pierreavital/
#   photo: speakers/Alex-Afanasyev.jpg
  bio: "Pierre Avital received his PhD in Signal Processing from the University of Paris Saclay in 2021, in cooperation with Valeo where he worked as a Research Engineer from 2017. He joined ZettaScale as a Research Engineer in 2021, working on providing clearer APIs for Zenoh while improving the core’s performance."

- name: Carlos Guimarães
  affiliation: ZettaScale Technology
  homepage: https://www.linkedin.com/in/carlos-guimar%C3%A3es-57276b31/
#   photo: speakers/Alex-Afanasyev.jpg
  bio: "Carlos Guimarães received the M.Sc. degree in computer and telematics engineering from the Universidade de Aveiro (Portugal) in 2011, and the Ph.D. degree in computer science, in 2019, under the scope of MAP-i Doctoral Program (Portugal). He is currently a Senior Technologist at ZettaScale Technology SARL (France), targeting the usage of Zenoh in embedded systems. Prior to that, he had worked as a Postdoctoral Researcher at Universidad Carlos III de Madrid (Spain)."

- name: Julien Enoch
  affiliation: ZettaScale Technology
  homepage: https://www.linkedin.com/in/julienenoch/
#   photo: speakers/Alex-Afanasyev.jpg
  bio: "Julien Enoch received his Master's degree in Computer Engineering at the University of Paris-Saclay, France, in 2000. Since then he acquired a great expertise in distributed systems, working on architectures and developments of various middleware technologies such as CORBA or DDS, and supporting their usage in various domains such as defense, transportation or robotic. Since 2018, he actively contributes to the Zenoh open-source project."

- name: Julien Loudet
  affiliation: ZettaScale Technology
  homepage: https://www.linkedin.com/in/jldt/
#   photo: speakers/Alex-Afanasyev.jpg
  bio: "Julien Loudet received his PhD in Computer Science from the University of Paris Saclay in 2019. Since 2016, he has been working on Distributed Systems, focusing on how to preserve the privacy of users. He joined ZettaScale as a Research Engineer in 2021 where he prominently works on Zenoh-Flow."

- name: Gabriele Baldoni
  affiliation: ZettaScale Technology
  homepage: https://www.linkedin.com/in/gbaldoni/
#   photo: speakers/Alex-Afanasyev.jpg
  bio: "Gabriele Baldoni received his Bachelor’s and Master’s degree in Computer Engineering and Telecommunication Engineering at the University of Catania, Italy, in 2015 and 2017, respectively. From 2017, he works as research engineer at ZettaScale, prominently targeting Zenoh-Flow. Starting from 2020, he is a PhD Student at University Carlos III of Madrid (UC3M), focusing is end-to-end applications in the Cloud-to-Thing continuum."

- name: William Liang
  affiliation: ADLINK
  homepage: https://www.linkedin.com/in/wyliang/
#   photo: speakers/Alex-Afanasyev.jpg
  bio: "William Liang received his PhD in Computer Science and Information Engineering from National Taiwan University in 1998. He was an assistant professor in National Taipei University of Technologies and then served in several companies in the industry such as Foxconn, ADLINK and some startups. His research domain and expertise covers parallel and distributed systems, embedded systems, computer architecture and operating systems. He is now a member of the Zenoh development team."

---

## {{ page.title }}

### Overview
* TOC
{:toc}

### Tutorial Program
{% assign abstractTitle="" %}
{% assign expanded=true %}
{% include program-online.html type="tutorial-zenoh" %}

### Introduction

Information-Centric solutions, also known as data-centric solutions, have been proposed and researched over the last decade without truly seeing adoption from the industry. Instead, the industry still heavily relies on “non-native” data-centric solutions, like MQTT or DDS, that emulate a data-centric behavior tied to the limitations of host-centric solutions, making them sub-optimal or inefficient. In addition, current solutions are typically targeting a single communication paradigm (either pub/sub or req/rsp) or a specific segment of the Cloud-to- Thing continuum.

**Eclipse Zenoh** aims at offering an open-source data-centric solution adapted to the industry. It unifies data in motion, data in-use, data-at-rest, and computations by carefully blending traditional pub/sub with geo-distributed storages. At the same time, it retains a level of time and space efficiency that is well beyond any of the mainstream offers. Zenoh provides a stack designed to (1) minimize network overhead, (2) support both extremely constrained devices, and powerful applications in the cloud, (3) support devices with low duty-cycle by allowing the negotiation of data exchange modes and schedules, (4) provide a rich set of abstractions for distributing, querying, and storing data along the entire system, and (5) provide extremely low latency and high throughput. By doing so, Zenoh can target the most powerful as well as the smallest things, thus covering the whole Cloud-to-Thing continuum.

After several years of careful design and performance assessments, we consider that, in 2022, Zenoh is mature and ready for its next stage of dissemination. With clear contributions in the automotive (e.g., Indy Autonomous Challenge) and robotics (e.g., ROS2) sectors, boosted by to the fact that is completely open-source, Zenoh can become a de-facto solution on the ICN landscape. ACM ICN 2022, as the flagship conference on the topic, can help us reach an even higher audience of experts in data-centric solutions and networks in general, thus contributing to not only on-going research discussions but also for future developments. As open source, the research community will also benefit from such developments.

{% comment %}

<!-- ### Tutorial Description

This half-day tutorial is expected to run 3 hours including a 10-minute break in the middle. It will be mostly real-time presentations with a few pieces of recorded demonstrations.

#### Warming up (30 min)

We start the tutorial with an overview of NDN security concepts, the principal differences between today’s and NDN applications regarding their deployment requirements, as well as quickly introduce the concept of trust schema, the central piece of the tutorial.

#### Overview of Trust Schema (30+ minutes)

The basic concept of NDN trust schema was first introduced in [6].
Its goals are to define security policies that regulate data signing and verification.
The basic idea is to define such policies via formal relations between the names of keys and the names of data, applying rules and links to the namespace levels.
In this part of the tutorial we will explore in depth the concepts of the trust schema and how they are applied to secure the applications in our simple use case scenario.

#### Break (10 min)

#### Simplified Trust Schema in NDN-Lite (20+ min)

NDN-Lite is a framework to enable end user-controlled home IoT systems over NDN.
In this part we will showcase how NDN-Lite can realize home IoT apps via a pub-sub API, highlighting security features of the implementation.
Specifically, the developed pub-sub API is designed to hide all the cryptographic operation details, while being powered by name-based policies, a simplified realization of the trust schema.

#### Designing of a Simple Trust Schema for IoT (30 min)

In this part, we will use a simple IoT application as a demo case for securing NDN deployment.
Primarily we will use the new developments of the trust schema, but we also going to briefly introduce how similar can be accomplished (in limited capacity) with other library realizations.

#### Q & A (20 minutes)

In addition to addressing questions in real time during the tutorial, we will also use this dedicated Q & A session to cover the questions collected from the conference Slack channel that touch on broader scope or deserve deeper elaborations.
This session will also offer the audience opportunities to share their own work related to NDN API development and configuration challenges as well as solutions. -->

{% endcomment %}

### Presenters

{% assign expand=true %}
{% include presenters.html presenters=page.presenters %}

### REFERENCES
