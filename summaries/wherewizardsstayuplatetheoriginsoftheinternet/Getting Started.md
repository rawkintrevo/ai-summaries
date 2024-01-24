---
layout: page
title: Getting Started
date: 2024-01-24 18:50:11
---

[Back](./)


The difficulty of building a network that switched packets of bits and did so dynamically was a challenging task. Bob Kahn, a scientist, understood the complexity of this problem and contributed ideas to the ARPA network project. He believed that a small-scale experiment would not be sufficient to learn meaningful information, so he urged for a transcontinental network of at least nineteen nodes to be built. BBN won the contract to build the network, and Kahn initially planned to return to his own research work after Christmas. However, he decided to stick around for the implementation of the network.

The team responsible for building the network, known as the IMP Guys, consisted of engineers and pragmatists who knew how to solve practical problems and make things work. They had assembled at BBN and were led by Frank Heart. They understood the importance of functionality over elegance or beauty and focused on making tradeoffs to create a reliable computer system. Their goal was to make the IMPs (Interface Message Processors) as unobtrusive as possible, like a simple household socket or switch.

The construction of the network required both hardware and software development. Willy Crowther, one of the IMP Guys, was responsible for writing the software code for the IMPs. Assembly-language programming was necessary, which required precise instructions to carry out minute steps. Crowther had a unique ability to keep track of these detailed steps and often drew flowcharts to visualize the entire process. The software development was done using a PDP-1 computer to write the code and then transferring it to the Honeywell 516 computer where it was converted into machine language.

Meanwhile, the hardware development was led by Severo Ornstein, who designed high-speed I/O devices for the IMPs. The IMP team had to decide which network operations would be handled by the IMP software and which would be built into the hardware. They favored software solutions whenever possible to allow for more flexibility in making revisions in the future.

In February, BBN finalized its contract with Honeywell for the purchase of the DDP-516 computers that would serve as the IMPs. The machines were installed at BBN, and the programmers began writing the IMP software. They discovered that the code could be much shorter than expected, with only about six thousand words required. They also faced challenges in assembling the code using the Honeywell assembler, but eventually developed their own efficient assembler on a PDP-1 computer.

The IMP Guys focused on ensuring reliability and error control in the network. They incorporated a 24-bit checksum to detect errors in transmission and implemented error correction techniques. The IMPs were designed to handle error detection and correction in hardware, as software calculations would be too slow. The team also worked on building a robust system that could withstand failures and automatically restart in case of a power outage or program crash.

The IMP Guys maintained open communication among themselves and held informal design reviews to discuss progress and exchange ideas. They wrote technical notes to share their thoughts and findings, and everyone on the team knew everything that was happening. This collaborative approach helped them make important decisions and solve problems.

Meanwhile, Bob Kahn was responsible for drafting the host-to-IMP interface specification, which described how a host computer should communicate with an IMP. He faced challenges in finalizing the specification and ensuring it met the requirements of both BBN and the host sites. Eventually, a revised specification was agreed upon and provided a foundation for the host teams to build their own interfaces.

The network project faced additional challenges, including connecting multiple host computers to each IMP and resolving host-to-host communication issues. Frank Heart emphasized the importance of keeping the boundary between the IMP and the host responsibilities clear to avoid complications. The IMPs were designed to be messengers, responsible for packet routing and error detection, while the hosts would be responsible for processing the content of the messages.

As the project progressed, the IMP Guys worked long hours, often late into the night, to meet the deadlines. They were focused on building a robust and reliable network that would facilitate communication between host computers. The challenges of creating a functional and efficient network required their expertise and collaboration.

This summary provides a detailed overview of the challenges and progress of building the network and the contributions of the IMP Guys in developing the IMP software and hardware. Their dedication and expertise were essential in creating a reliable and efficient network infrastructure.

Words: 748