---
layout: default
title: "Half-day Tutorial: CCNx-based Cloud-Native Function: Networking and Applications"
group: Tutorials

presenters:
- name: Yusaku Hayamizu
  affiliation: National Institute of Information and Communications Technology (NICT)
#   homepage: https://users.cs.fiu.edu/~afanasyev
#   photo: speakers/Alex-Afanasyev.jpg
  bio: "Yusaku Hayamizu received his B.E., M.E., and Ph.D. degrees in engineering from Kansai University in 2014, 2016, and 2019, respectively. He is currently a researcher of Network Architecture Laboratory at National Institute of Information and Communications Technology (NICT). His research interests include computer networks, information centric networks, traffic control, in-network computing, and network softwarelization. Dr. Hayamizu is the recipient of Best Paper Awards from the 2017 IEEE CQR Workshop and the 2018 IEEE LANMAN Symposium. He is a member of the ACM, the IEEE, and the IEICE."

- name: Atsushi Ooka
  affiliation: National Institute of Information and Communications Technology (NICT)
#   homepage: https://users.cs.fiu.edu/~afanasyev
#   photo: speakers/Alex-Afanasyev.jpg
  bio: "Atsushi Ooka is a researcher of Network Architecture Laboratory at NICT. He received M.E. and Ph.D. degrees in the Graduate School of Information Science and Technology, Osaka University in 2014 and 2017, respectively. His research interests include the design and implementation of a router in content-centric networking. He is a member of the IEEE."

- name: Kazuhisa Matsuzono
  affiliation: National Institute of Information and Communications Technology (NICT)
#   homepage: https://users.cs.fiu.edu/~afanasyev
#   photo: speakers/Alex-Afanasyev.jpg
  bio: "Kazuhisa Matsuzono is a researcher of Network Architecture Laboratory at NICT. He received a Ph.D. from Keio University in fiscal 2012. He was a post-doctoral fellow at INRIA in 2013. His research interests include transport protocols for multimedia flows, network coding, and information-centric networks. He has been a vice-chair of IEICE Technical Committee on ICN from 2019. He is a member of the IEEE and IEICE."

- name: Hitoshi Asaeda
  affiliation: National Institute of Information and Communications Technology (NICT)
#   homepage: https://users.cs.fiu.edu/~afanasyev
#   photo: speakers/Alex-Afanasyev.jpg
  bio: "Hitoshi Asaeda is a director of Network Architecture Laboratory at NICT. He received a Ph.D. degree from Keio University. He was previously with IBM Japan, Ltd., a research engineer specialist at INRIA, France, and a project associate professor at Keio University. He was a guest editor-in-chief of the special series of IEICE Trans. Commun. in 2016 and a chair of IEICE Technical Committee on ICN from 2017 to 2019. He was a general co-chair of IEEE/ACM IWQoS 2021. His research interests include information-centric networking, network coding, high-quality streaming, and distributed computing. He received the IEICE Communications Society Outstanding Contributions Award in 2019. He is a senior member of IEEE and IEICE, and a member of ACM."

---

## {{ page.title }}

### Overview
* TOC
{:toc}

### Tutorial Program
{% assign abstractTitle="" %}
{% assign expanded=true %}
{% include program-online.html type="tutorial-cefore" %}

### Introduction

A dozen years has been passed since the concept of Information- Centric Networking (ICN) [1] had been originally advocated. Currently, the ICN has been forked to several concrete network architectures such as Content-Centric Networking (CCNx) [2, 3] and Named-Data Networking (NDN) [4], and studies on routing, forwarding, caching, security, etc, have been widely investigated by various research communities thus far. One missing piece might be a deployment solution of the developed ICN approaches into the existing Internet infrastructures.

The cloud-native ecosystem such as Docker [5] and Kubernetes [6] is emerging microservices technology for edge/fog computing. Docker container has lot of great benefits for operation and management of software resources, e.g. portability, performance, agility, and scalability. In this tutorial, we integrate the microservices technology with Cefore [7, 8] that is CCNx1.0-compliant software program enabling ICN communications for providing simple and quick construction and deployment of ICN networks and applications.

In our lecture-style half-day tutorial, we introduce the Cefore software platform and its integration with Docker technologies. We also explain a Python wrapper program named Cefpyco [9] that helps developing ICN applications running with Cefore. We finally demonstrate utilities delivered with Cefore software package and several sample applications.

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
[1] V. Jacobson, et al., “Networking Named Content,” in Proc. ACM
CoNEXT’09, vol. E102-B, no. 9, Sept. 2019.

[2] “Content-Centric Networking (CCNx) Semantics,” https://datatracker.
ietf.org/doc/rfc8569/ , Accessed on 7 July 2022.

[3] “Content-Centric Networking (CCNx) Messages in TLV Format,” https:
//datatracker.ietf.org/doc/rfc8609/ , Accessed on 7 July 2022.

[4] L. Zhang, et al., “Named Data Networking,” ACM SIGCOMM CCR, vol.
44, no. 3, pp 66-73, July 2014.

[5] “Docker,” https://www.docker.com/, Accessed on 7 July 2022.

[6] “Kubernetes,” https://kubernetes.io/ , Accessed on 7 July 2022.

[7] “Cefore,” https://cefore.net , Accessed on 7 July 2022.

[8] H. Asaeda, et al., “Cefore: Software Platform Enabling Content-Centric
Networking and Beyond,” IEICE Trans. Commun., vol.E102-B, no.9,
pp.1792-1803, Sept. 2019.

[9] “Cefpyco”, https://github.com/cefore/cefpyco, Accessed on 7 July 2022.

[10] H. Asaeda, et al., “CCNinfo: Discovering Content and Network Information
in Content-Centric Networks,” IRTF Internet-Draft, draft-irtficnrg-
ccninfo-10 (work in progress), Apr. 2022.