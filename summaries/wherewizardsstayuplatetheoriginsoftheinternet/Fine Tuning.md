---
layout: page
title: Fine Tuning
date: 2024-01-24 18:51:04
---

[Back](./)


In the second year of the network, changes were implemented to improve reliability and reduce costs. The decision was made to replace the Honeywell 516 with the newer, less expensive Honeywell 316, as the ruggedized version of the 516 was deemed unnecessary and hindered routine maintenance tasks. However, Honeywell was slow to adapt to BBN's vision for the network and there were issues with prolonged hardware failures. Ben Barker, who maintained the IMPs, proposed building a BBN-directed maintenance team, but this was initially opposed by McKenzie due to concerns about Barker's messy office. Eventually, Barker was given the job and implemented a crack maintenance team.

Meanwhile, Heart's confidence in the network's reliability grew and plans were made to transition to a new 316-based IMP. This transition was part of a larger shift in the network to allow for more users without the need for a host computer. This would open up the network to a wider range of users, aligning with Licklider's vision of a computer network facilitating communication and interaction.

To support this shift, a new terminal controller, called a Terminal IMP or TIP, needed to be built. This device would allow for multiple terminal lines to be connected directly to the IMP and the network. BBN accelerated the development of the TIP and within six months, two prototype machines based on the 316 were completed.

BBN also continued to improve the packet-switching technology and tested various routing algorithms, flow-control schemes, and throughput. The Network Control Center expanded and became staffed around the clock to maintain the network. An automatic phone dialer was added to monitor the condition of modems in the network. During one test, an angry voice on the other end of the line criticized a technician for calling with a whistle.

Congestion control was addressed by redesigning the scheme to reserve enough space in the IMP memory buffers for reassembly of incoming packets. This prevented the insertion of more traffic into the network than the destination IMP could handle.

BBN also became more involved in the work of the Network Working Group (NWG), participating in committees working on protocols such as Telnet and FTP. Telnet allowed for basic communication between two host machines, while FTP facilitated file transfers between machines. The FTP working group, led by Abhay Bhushan, developed a file-transfer protocol that could handle the differences between various machines on the network.

In July 1972, the final version of FTP was released as RFC 354, marking another milestone in the development of the network.

Overall, the second year of the network saw improvements in reliability, cost-effectiveness, and user accessibility. The network continued to grow and evolve, bringing Licklider's vision of a connected world one step closer to reality.

Words: 453