---
layout: page
title: GPT Understands, Too
date: 2023-11-03 21:05:05
---

[Back](./)


The paper introduces a novel method called P-Tuning, which utilizes trainable continuous prompt embeddings in conjunction with discrete prompts to improve the performance and stability of language model adaptation. The authors identify a problem with manual discrete prompts, which tend to lead to unstable performance, as even a slight change in the prompt can result in a significant drop in performance. They propose using continuous prompts to minimize the impact of changes in discrete prompts and enhance training stability. The continuous prompts are updated through backpropagation to optimize the task objective. Additionally, a prompt encoder using LSTMs or MLPs models the dependency between continuous prompt embeddings. 

The authors conduct experiments on two NLU benchmarks: LAMA and SuperGLUE. With a frozen language model, P-Tuning outperforms both manual discrete prompts and searched prompts by a significant margin on LAMA. On SuperGLUE, with the language model finetuned, P-Tuning surpasses PET with the best discrete prompts under both the fully-supervised and few-shot settings. The results demonstrate that P-Tuning not only improves performance but also reduces the performance gap between different prompts, enhancing stability for language model adaptation.

The paper also addresses the issue of stability in language model adaptation. The authors show that manual prompts often yield volatile results, while appending trainable continuous prompts to manual prompts can stabilize their performances. They observe that the performance gap between different prompts is more prominent in few-shot learning, but P-Tuning helps improve the performance of poorly performing patterns and reduces the standard deviation, thereby increasing stability.

The authors compare P-Tuning with other approaches in the field of language model prompting. They note that P-Tuning differs from previous methods by utilizing continuous prompt embeddings, which are shown to complement discrete prompts. Concurrent works have also proposed using continuous prompts, but they focus on natural language generation tasks, whereas P-Tuning is designed for NLU tasks. The authors also mention other works that aim to improve knowledge probing, as well as studies on the knowledge learned by language models.

In conclusion, the paper introduces P-Tuning, a method that combines trainable continuous prompt embeddings with discrete prompts to improve the performance and stability of language model adaptation. The experiments demonstrate that P-Tuning outperforms other approaches on NLU benchmarks and increases stability in language model adaptation. The paper contributes to the field of language model prompting and provides insights into the effectiveness of continuous prompts for NLU tasks.

Words: 397