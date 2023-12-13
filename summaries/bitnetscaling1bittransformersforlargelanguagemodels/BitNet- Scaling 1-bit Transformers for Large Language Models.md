---
layout: page
title: BitNet- Scaling 1-bit Transformers for Large Language Models
date: 2023-12-13 17:30:59
---

[Back](./)


In this paper, the authors propose BitNet, a scalable and stable 1-bit Transformer architecture designed for large language models. They address the challenges posed by the increasing size of large language models, such as deployment and environmental impact due to high energy consumption. BitNet aims to reduce memory footprint and energy consumption while maintaining competitive performance.

The authors introduce BitLinear as a replacement for the nn.Linear layer in the Transformer in order to train 1-bit weights from scratch. They conduct experiments on language modeling and compare BitNet to state-of-the-art 8-bit quantization methods and FP16 Transformer baselines. The results show that BitNet achieves competitive performance while significantly reducing memory footprint and energy consumption. They also show that BitNet follows a scaling law similar to full-precision Transformers, suggesting its potential for effective scaling to even larger language models.

The authors also discuss the advantages of quantization-aware training compared to post-training quantization methods. While post-training quantization is simple and easy to apply, it often leads to a loss of accuracy, especially with lower precision. Quantization-aware training, on the other hand, results in better accuracy as the model is trained to account for the reduced precision from the beginning. BitNet is the first work to investigate quantization-aware training for 1-bit large language models.

Quantization methods are evaluated on various benchmarks, including Winogrande, Winograd, Storycloze, and Hellaswag. BitNet achieves competitive performance compared to the baselines, particularly for lower bit levels. The authors also analyze the zero-shot and few-shot performance of BitNet and the baselines on downstream tasks. BitNet consistently outperforms the baselines, especially at lower bit levels. The results demonstrate the effectiveness of quantization-aware training for 1-bit large language models.

The authors also conduct an ablation study to analyze the choices made in the BitNet architecture. They compare different activation quantization methods, including absmax and the elastic function, and find that absmax performs better. They also compare SubLN with Pre-LN and the BMT architecture for training stability, and find that SubLN out

Words: 327