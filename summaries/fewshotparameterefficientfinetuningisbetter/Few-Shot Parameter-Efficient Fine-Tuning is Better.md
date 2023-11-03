---
layout: page
title: Few-Shot Parameter-Efficient Fine-Tuning is Better
date: 2023-11-03 21:21:01
---

[Back](./)


The paper presents a comparison between few-shot parameter-efficient fine-tuning (PEFT) and few-shot in-context learning (ICL) for pre-trained language models. The authors show that PEFT offers better accuracy and significantly lower computational costs compared to ICL. They also introduce a new PEFT method called (IA)3, which scales activations by learned vectors to improve performance while introducing only a small number of new parameters.

The paper begins by discussing the background of pre-trained language models and their use in fine-tuning for downstream tasks. Fine-tuning requires updating all model parameters for each new task, which can be computationally expensive when fine-tuning on multiple tasks. ICL, on the other hand, enables a model to perform a new task by inputting a small number of prompted examples without gradient-based training. ICL has gained recent interest but has drawbacks such as high computational costs and lower performance compared to fine-tuning.

The authors propose a recipe called T-Few, which combines the T0 model (a variant of T5) with the (IA)3 PEFT method. T-Few achieves strong performance on novel, unseen tasks while updating only a small fraction of the model's parameters. The authors also introduce additional loss terms to improve performance on classification and multiple-choice tasks.

To evaluate the effectiveness of T-Few, the authors compare it to strong ICL baselines on various datasets. They find that T-Few outperforms ICL methods, even when using larger models. They also show that T-Few achieves super-human performance on the RAFT benchmark, outperforming the state-of-the-art by a large margin.

The paper provides a detailed analysis of the computational, memory, and storage costs of T-Few. They find that T-Few uses significantly fewer FLOPs during inference compared to ICL methods, and the training time is relatively short. The storage cost of T-Few is larger due to the additional parameters introduced by (IA)3, but it is still relatively small compared to the model checkpoints themselves.

In conclusion, the authors present T-Few as a parameter-efficient few-shot learning recipe that achieves better accuracy and lower computational costs compared to ICL methods. They demonstrate the effectiveness of T-Few on various datasets and achieve super-human performance on the RAFT benchmark. The paper provides valuable insights into the benefits of PEFT and offers a new perspective on few-shot learning with large language models.

Words: 372