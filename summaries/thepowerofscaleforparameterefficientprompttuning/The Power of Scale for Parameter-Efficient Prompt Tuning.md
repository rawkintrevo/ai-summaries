---
layout: page
title: The Power of Scale for Parameter-Efficient Prompt Tuning
date: 2023-11-03 20:50:32
---

[Back](./)


In this paper, the authors explore the concept of "prompt tuning" as a mechanism for adapting frozen language models to perform specific downstream tasks. They introduce the idea of "soft prompts," which are learned through backpropagation and can be tuned to incorporate signals from labeled examples. The authors compare this approach to the discrete text prompts used by GPT-3 and show that prompt tuning outperforms GPT-3's few-shot learning by a large margin.

The authors also demonstrate that as model size increases, prompt tuning becomes more competitive with model tuning. They use the T5 model to conduct ablations on model size and show that prompt tuning "closes the gap" and matches the performance of model tuning when models exceed billions of parameters. This is significant because large models are costly to share and serve, and the ability to reuse one frozen model for multiple downstream tasks can alleviate this burden.

Prompt tuning is presented as a simplification of the recently proposed "prefix tuning." While prefix tuning involves freezing the model parameters and backpropagating the error to prefix activations, prompt tuning only allows for the tuning of prompt parameters. The authors compare prompt tuning to other similar approaches, such as manual prompt design and non-differentiable search methods, and show that prompt tuning is more effective.

The authors also investigate the benefits of conditioning a frozen model with soft prompts, including improved robustness to domain transfer and efficient prompt ensembling. They demonstrate that prompt tuning outperforms model tuning on zero-shot domain transfer tasks, where the distribution of inputs differs between training and evaluation. They also show that ensembling multiple prompt adaptations of a pre-trained language model is more efficient than ensembling multiple tuned models.

In terms of interpretability, the authors examine the learned soft prompts and find that the nearest neighbors to the prompt tokens form semantic clusters. They also observe that when initializing the prompts with class labels, the labels often persist through training, suggesting that the model learns to store the expected output classes in the prompts. However, when examining longer prompts, the authors find that there may be excess capacity or difficulty in localizing information to specific positions.

In conclusion, prompt tuning is presented as a competitive technique for adapting frozen pre-trained language models to downstream tasks. It offers the benefits of reduced storage and serving costs, efficient multi-task serving, and improved generalization to new domains. The authors believe that separating task-defining parameters from general language-modeling parameters opens up new research opportunities in the field.

Words: 415