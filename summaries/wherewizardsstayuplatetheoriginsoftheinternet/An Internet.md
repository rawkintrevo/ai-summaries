---
layout: page
title: An Internet
date: 2024-01-24 20:20:34
---

[Back](./)


This excerpt provides a detailed account of the collaboration between Bob Kahn and Vint Cerf to create a seamless connection among different computer networks. It begins by explaining how Kahn and Cerf met during testing at UCLA in 1970, and how they both became interested in the challenge of connecting different networks together. They came up with the idea of a "gateway," a routing computer that would sit between various networks and transfer messages between them. The gateway would need to appear as a regular host to each network, despite the differences in interfaces, packet sizes, and transmission rates.

The next challenge was packet transmission and reliability. Each network operated under its own rules, so the International Network Working Group had to devise protocols that could cope with these differences while allowing hosts on different networks to communicate. They decided to replace the host-to-host Network Control Protocol with a more independent protocol that shifted the responsibility of reliability from the network to the destination hosts. The goal was to achieve end-to-end reliability, with the network only responsible for delivering packets to their destination.

Once the conceptual framework was established, Kahn and Cerf spent several months in 1973 working out the details. They held a seminar at Stanford to discuss the development of the host-to-host protocol, and they collaborated on a paper titled "A Protocol for Packet Network Intercommunication," which was published in 1974. This paper described the concept of encapsulating messages in "data-grams" and introduced the idea of gateways reading only the envelope of the messages. The paper also addressed the reliability issues and proposed that the network should only be responsible for delivering packets, while the hosts should handle reassembling and error recovery.

The invention of TCP (Transmission Control Protocol) was crucial to networking, as it enabled communication across networks. With TCP, anyone could build a network and as long as there was a gateway computer to interpret and route packets, the network could communicate with any other network. The potential power of TCP began to be recognized, and it became clear that networking had a future beyond the experimental ARPANET.

As more resources became available over the ARPANET, its usage began to increase. Net traffic grew to an average of 3.2 million packets per day by August 1973, and the Net expanded at a rate of about one new node per month from 1973 to 1975. However, there was an imbalance between resource providers and customers, so DARPA introduced terminal IMPs to help balance the demand.

The ARPANET also began to attract users from diverse fields who wanted to access the network's resources. Large databases, such as the Computer Corporation of America's Datacomputer, became popular, and researchers used the network for tasks like medical studies and mental health program evaluations. SRI established the ARPANET News to provide information to users, and the newsletter helped create a sense of community among the growing user base. However, communication and accessing resources over the ARPANET remained cumbersome, and there was a demand for higher-level application programs to make it easier for users to tap into available resources.

In addition to these advancements, the excerpt also mentions the tensions and challenges faced by DARPA and the ARPANET. There were concerns about the network's military applications and connections to the Pentagon, as well as allegations of improper use of the ARPANET by Army intelligence. These instances raised questions and required DARPA to explain how the ARPANET was being used.

Overall, this excerpt provides a detailed account of the collaboration between Kahn and Cerf, the challenges they faced in designing the protocol for packet network intercommunication, and the growing usage and impact of the ARPANET.

Words: 611