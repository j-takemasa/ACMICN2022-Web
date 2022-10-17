---
layout: default
title: "One-day Tutorial: Evaluating NDN using ndnSIM and Mini-NDN"
group: Tutorials

presenters:
- name: Alex Afanasyev
  affiliation: Florida International University
#   homepage: https://users.cs.fiu.edu/~afanasyev
#   photo: speakers/Alex-Afanasyev.jpg
  bio: "Alex Afanasyev is an Assistant Professor in Florida International University, Miami. He received his Ph.D. degree in computer science from UCLA in 2013. His research focus is on the next-generation Internet architecture as part of the Named Data Networking (NDN) project. His research interests include a variety of topics that are vital for the success of NDN, including scalability of name-based routing, auto-configuration, distributed data synchronization, application and network security. Dr. Afanasyev is also leading the development effort of the overall NDN codebase."

- name: Saurab Dulal
  affiliation: University of Memphis
#   homepage: https://users.cs.fiu.edu/~afanasyev
#   photo: speakers/Alex-Afanasyev.jpg
  bio: "Saurab Dulal is a Ph.D. student at the University of Memphis, Tennessee. He received his M.S. degree in Computer Science from The University of Memphis, in Dec 2020, and a Bachelor’s Degree in Computer Engineering from the Tribhuvan University, Nepal, in 2014. His research interest involves information-centric networking, especially NDN and Distributed Computing. He is involved in various NDN research topics such as security, IoT, data synchronization, routing, and forwarding."

- name: Varun Patil
  affiliation: University of California, Los Angeles
#   homepage: https://users.cs.fiu.edu/~afanasyev
#   photo: speakers/Alex-Afanasyev.jpg
  bio: "Varun Patil is a Ph.D. student at the University of California, Los Angeles. He received his M.S. degree in Computer Science from UCLA, in Dec 2021, and a Bachelor’s Degree in Mechanical Engineering from the Indian Institute of Technology, Bombay, in 2020. His research interest involve NDN with a focus on synchronization protocols and distributed systems, and is involved in projects such as State Vector Sync and development of distributed storage systems over NDN."

- name: Beichuan Zhang
  affiliation: University of Arizona
#   homepage: https://users.cs.fiu.edu/~afanasyev
#   photo: speakers/Alex-Afanasyev.jpg
  bio: "Beichuan Zhang is an Associate Professor at the Department of Computer Science, the University of Arizona. His research interest is in Internet routing architectures and protocols. He has been working on Named Data Networking, green networking, and inter-domain routing. He received the Applied Networking Research Prize in 2011 by ISOC and IRTF, and best paper awards at IEEE ICDCS in 2005 and IWQoS in 2014. Dr. Zhang received Ph.D. from UCLA and B.S. from Peking University."

- name: Lixia Zhang
  affiliation: University of California, Los Angeles
#   homepage: https://users.cs.fiu.edu/~afanasyev
#   photo: speakers/Alex-Afanasyev.jpg
  bio: "Lixia Zhang is a Professor in the Computer Science Department of UCLA. She received her Ph.D in computer science from MIT and was a member of the research staff at Xerox PARC before joining UCLA. She is a fellow of ACM and IEEE, the recipient of IEEE Internet Award and ACM SIGCOMM Lifetime Achievement Award, and the holder of UCLA Postel Chair in Computer Science. Since 2010 she has been leading the effort on the design and development of the NDN architecture."

---

## {{ page.title }}

### Overview
* TOC
{:toc}

### Tutorial Program
{% assign abstractTitle="" %}
{% assign expanded=true %}
{% include program-online.html type="tutorial-ndn" %}

### Introduction
As the Named Data Networking (NDN) architecture [2, 4, 7] is still under active development, it is important to master the evaluation tools that can be used to measure different design proposals and their various tradeoffs. Two popular NDN evaluation tools have emerged over the years. One is ndnSIM, an NS-3 based network simulator [1, 5], which continuously tracks the NDN architecture updates with the prototype NDN forwarder implementation (NFD [3]). The other tool, is Mini-NDN [6], a Mininet-based emulator, which allows users to perform experimentation with the real code in an emulated environment. This tutorial aims to help the audience gain knowledge and experience of both tools. More specifically, the tutorial will start with a brief introduction of both ndnSIM and Mini-NDN, then moving on to explain in detail their similarities and differences, which one to use for what kinds of evaluation. The tutorial will guiade the audience to go through several straw-man examples of simulation and emulation scenarios.

### Tutorial Description
This full day tutorial is expected to last a total of 7 hours, including two 10-minute breaks and one hour lunch break in the middle. It will be a mix of presentations, real-time coding, pre-recorded demonstrations, and (depending on participants) real time dive-ins into specific aspects of simulation and emulation scenarios. After the initial introduction, the rest of morning session will be devoted to ndnSIM and the afternoon to Mini-NDN.

{% comment %}
{% endcomment %}

### Presenters

{% assign expand=true %}
{% include presenters.html presenters=page.presenters %}

### REFERENCES
[1] Alexander Afanasyev, Ilya Moiseenko, and Lixia Zhang. 2012. ndnSIM:
NDN simulator for NS-3. Technical Report NDN-0005. NDN. http:
//named-data.net/techreports.html

[2] Alexander Afanasyev, Tamer Refaei, Lan Wang, and Lixia Zhang. 2018.
A Brief Introduction to Named Data Networking. In Proc. of MILCOM.

[3] Alexander Afanasyev, Junxiao Shi, Beichuan Zhang, Lixia Zhang, Ilya
Moiseenko, Yingdi Yu, Wentao Shang, Yanbiao Li, Spyridon Mastorakis,
Yi Huang, Jerald Paul Abraham, Eric Newberry, Steve DiBenedetto,
Chengyu Fan, Christos Papadopoulos, Davide Pesavento, Giulio Grassi,
Giovanni Pau, Hang Zhang, Tian Song, Haowei Yuan, Hila Ben Abraham,
Patrick Crowley, Syed Obaid Amin, Vince Lehman, Muktadir
Chowdhury, and Lan Wang. 2018. NFD Developer’s Guide. Technical
Report NDN-0021, Revision 8. NDN. http://named-data.net/techreports.
html

[4] Van Jacobson, Diana K Smetters, JD Thronton, Michael F Plass,
Nicholas H Briggs, and RL Braynard. 2009. Network Named Content.
In Proc. of CoNEXT.

[5] Spyridon Mastorakis, Alexander Afanasyev, Ilya Moiseenko, and Lixia
Zhang. 2016. ndnSIM 2: An updated NDN simulator for NS-3. Technical
Report NDN-0028, Revision 2. NDN.

[6] Mini-NDN. 2022. Mini-NDN: A Mininet-based NDN emulator. Online:
https://minindn.memphis.edu.

[7] Lixia Zhang, Alexander Afanasyev, Jeffrey Burke, Van Jacobson, Patrick
Crowley, Christos Papadopoulos, LanWang, Beichuan Zhang, et al. 2014.
Named data networking. ACM SIGCOMM Computer Communication
Review 44, 3 (2014), 66–73.