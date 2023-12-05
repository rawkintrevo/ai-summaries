---
layout: page
title: Measuring the Effects of Data Parallelism on Neural Network Training
date: 2023-12-05 19:31:12
---

[Back](./)


The introduction discusses the advancements in neural networks and their effectiveness in various prediction tasks. It mentions that while hardware improvements have enabled training larger models on larger datasets, training time still limits the predictive performance and application of these techniques. The introduction highlights the importance of faster training in improving model quality, facilitating experimentation, and enabling frequent model updates. 

Data parallelism is described as a popular approach to accelerate neural network training. It involves distributing training examples across multiple processors to compute gradient updates and aggregating these updates. Data parallelism is model-agnostic and applicable to any neural network architecture. The introduction also mentions model parallelism, which involves distributing parameters and computation across different processors for the same training examples. 

The discussion then focuses on the increasing capacity for data parallelism in neural network training due to advances in hardware, such as GPUs and custom ASICs. The benefits and costs of data parallelism in large-scale systems are not yet well studied, and there is a range of hypotheses and empirical results in the literature. The introduction emphasizes the need for a comprehensive experimental study on the effects of data parallelism on neural network training. 

The scope of the study is defined to focus on variants of mini-batch stochastic gradient descent (SGD), which are the dominant algorithms for training neural networks. The study considers synchronous SGD due to its popularity and advantages over asynchronous SGD. The primary concern of practitioners is out-of-sample error and the cost required to achieve it, which can be measured in terms of training time and hardware costs. The number of training steps is identified as the main measure of training cost, as it is hardware-agnostic and can be used to compute total costs for any hardware. 

The introduction concludes by outlining the most important questions that need to be explored to understand the costs and benefits of data parallelism with mini-batch SGD and its variants. These questions include the relationship between batch size and number of training steps to reach a goal out-of-sample error, the factors governing this relationship, and the potential cost of using large batch sizes in terms of out-of-sample error.

Words: 357