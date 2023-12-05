---
layout: page
title: FEDPARA: LOW-RANK HADAMARD PRODUCT FOR COMMUNICATION-EFFICIENT FEDERATED LEARNING
date: 2023-12-05 20:57:52
---

[Back](./)


In this work, the authors propose a communication-efficient parameterization method called FedPara for federated learning. The method re-parameterizes weight parameters of layers using low-rank weights followed by the Hadamard product. The authors compare FedPara to conventional low-rank parameterization and show that FedPara has a larger capacity and can achieve comparable performance with 3 to 10 times lower communication costs. They also extend FedPara to a personalized federated learning application called pFedPara, which separates parameters into global and local ones. The authors demonstrate that pFedPara outperforms competing personalized FL methods with fewer parameters.

Federated learning (FL) is a collaborative learning strategy that allows leveraging local computing resources of edge devices without sharing data. However, FL faces challenges with heterogeneous data and systems, as well as communication overheads. The authors propose FedPara to overcome these challenges. They show that FedPara reduces communication costs while maintaining a large capacity by using a low-rank Hadamard product parameterization. The authors also demonstrate that FedPara can be combined with other FL optimizers to improve communication efficiency further.

The authors evaluate FedPara and pFedPara on various network architectures and datasets. They compare their methods to the original models and conventional low-rank parameterization. The authors show that FedPara achieves higher ranks and better performance than low-rank parameterization. They also show that pFedPara outperforms competing personalized FL methods. The authors further analyze the capacity, communication costs, and compatibility of their methods.

The authors discuss potential issues with FedPara, such as gradient instability and computational cost. They suggest future research directions to address these issues and improve the computation and communication efficiency of FedPara in large-scale distributed learning scenarios.

Overall, the paper presents a novel method for communication-efficient federated learning and demonstrates its effectiveness through experiments. The proposed method shows promise for reducing communication costs while maintaining performance in FL.

Words: 300