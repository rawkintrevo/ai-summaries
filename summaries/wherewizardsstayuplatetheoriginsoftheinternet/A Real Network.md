---
layout: page
title: A Real Network
date: 2024-01-24 20:19:31
---

[Back](./)


In October 1969, the second Interface Message Processor (IMP) was installed at SRI, following the successful installation of the first IMP at UCLA. Bob Taylor, who had been heavily involved in the network project, left ARPA and took a post at the University of Utah. The IMP installation at SRI was a significant milestone as it allowed for the connection of two disparate computers.

The SRI team, similar to the UCLA team, had to scramble to get ready for the arrival of the IMP. However, unlike the UCLA team, the SRI team loved their host computer, an SDS 940, because it was more fun to program. Bill Duvall, an SRI researcher, wrote a program that made the 940 think it was communicating with a dumb terminal, which was an interim solution to the host-to-host communication problem.

Once both IMPs were installed and the hosts were running, the researchers were able to test the actual two-node ARPA network. The first thing they had to do was to connect to each other. They used a phonelike box attached to the IMPs to initiate the connection. The connection quality was not very good, and there were some technical difficulties, but eventually, they were able to establish a successful connection.

It is ironic that the first program used over the network was one that made the distant computer act as a terminal, as the whole purpose of the network was to eliminate the master-slave relationship. However, this was a familiar use case that helped build trust in the new technology.

Impressively, by the end of 1969, a four-node network had been established, connecting UCLA, SRI, UC Santa Barbara, and Utah. However, there were some vulnerabilities in the network structure. For example, there was no direct link between UCLA and Utah, or between Santa Barbara and Utah, so if the SRI IMP crashed, Utah would be cut off from the network.

There were also disruptions caused by users not realizing the consequences of their actions on the network. At Santa Barbara, the students treated the IMP as a toy and would turn it on and off, disrupting network traffic analysis and experiments being conducted by researchers at BBN and UCLA.

By the end of 1969, the Network Working Group (NWG) had not yet developed a host-to-host protocol. Under pressure to show progress, they presented a patched-together protocol called Telnet, which allowed for remote log-ins, but did not solve the problem of two computers working together. The NWG went back to the drawing board and, after a year of meetings and several RFCs, they produced a complete protocol called the Network Control Protocol (NCP).

In January 1970, Bob Kahn decided to test various scenarios in which the network could suffer congestive failure. He flew to Los Angeles and worked with Dave Walden to put the network through its paces. They were able to induce a network lockup by overwhelming the IMPs with packets, proving Kahn's hypothesis. Despite this setback, the hardware and software of the network were working well, and ARPA's unique approach to the project had been successful.

Overall, the predictions of failure were proven wrong, and the network experiment was a resounding success.

Words: 529