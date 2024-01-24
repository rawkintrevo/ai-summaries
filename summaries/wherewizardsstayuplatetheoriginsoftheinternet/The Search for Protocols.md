---
layout: page
title: The Search for Protocols
date: 2024-01-24 18:50:39
---

[Back](./)


In the summer of 1968, a group of graduate students from UCLA, SRI, UC Santa Barbara, and the University of Utah met to discuss the networking experiment being planned by ARPA. They were excited about the prospects of networking and imagined various possibilities such as interactive graphics, cooperating processes, automatic database query, and electronic mail. However, they lacked concrete details about how the network would be implemented and how hosts would communicate with each other.

To address these questions, the group decided to meet regularly and discuss their ideas. Since there were no official protocol designers at the time, Steve Crocker volunteered to write the first minutes of their discussions. He titled it "Request for Comments" (RFC) and sent it out on April 7, 1969, to the other sites. The RFC described the basic handshake between two computers and became the first of many RFCs that would be used to promote cooperation and open expression in the computer networking community.

The group started calling themselves the Network Working Group (NWG) and focused on designing protocols for host-to-host communication. They wanted to create a common base that would be simple, flexible, and adaptable to future needs. They adopted a layered approach to protocol design, with each layer having limited scope and the expectation that they could be combined or modified as needed.

One of the main challenges in designing the host-to-host protocol was getting the computers to communicate as equals, rather than one being the master and the other the subordinate. The computers of that time were egocentric and not designed for peer-to-peer communication. The NWG aimed to create protocols that would allow the mainframe computers to engage in simple dialogues with each other.

As the NWG worked on designing the protocol, they also had to write network applications for specific tasks such as remote log-ins and file transfers. They received a set of specifications for connecting host computers to the Interface Message Processors (IMPs) from BBN, the company responsible for building the network. However, the specifications did not include any special software for host-to-host communication, leaving it up to the host computers to figure out.

In the summer of 1969, as the first IMP was about to arrive at UCLA, the NWG was still struggling to finalize the host-to-host protocol. They decided to tell each site to create makeshift protocols in the meantime. UCLA managed to build the hardware interface for their host-to-IMP connection, thanks to the efforts of graduate student Mike Wingfield.

The IMP was shipped to UCLA by air freight and arrived on August 30, 1969, two days earlier than expected. Len Kleinrock, Steve Crocker, Jon Postel, Vint Cerf, and others were present to receive the IMP. It was larger than expected, roughly the size of a refrigerator, and weighed over nine hundred pounds. The IMP was swiftly installed and connected to the host computer, and within an hour, data was being transmitted between the Sigma-7 and the IMP.

Although there were concerns about synchronizer bugs, everything seemed to be working smoothly. Ben Barker, who accompanied the IMP to UCLA, called Frank Heart, the project leader, to inform him that the IMP was successfully connected and communicating with the host computer. Heart advised Barker to stay a few more days to ensure nothing went wrong, but the IMP continued to function perfectly.

Thus, the arrival of the IMP at UCLA marked a milestone in the development of the ARPANET, and the NWG continued their work on designing protocols and applications for the emerging network.


Words: 586