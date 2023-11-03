---
layout: page
title: LLM int8()- 8-bit Matrix Multiplication
date: 2023-11-03 21:16:45
---

[Back](./)


The paper discusses a new procedure for the quantization of large language models (LLMs) that reduces the memory required for inference while maintaining full precision performance. The authors introduce LLM.int8(), a two-part quantization procedure that allows the conversion of a 175B parameter LLM into an 8-bit format that can be used immediately without performance degradation. This method is achieved by understanding and working around the properties of highly systematic emergent features in transformer language models.

The paper begins by highlighting the memory requirements of LLMs and the importance of reducing the size of parameters through quantization. Previous 8-bit quantization methods have shown to reduce memory use but often require further tuning and have only been studied for models with less than 350M parameters. The authors aim to address the challenge of quantizing LLMs with billions of parameters without performance degradation.

The proposed method, LLM.int8(), consists of vector-wise quantization and mixed-precision decomposition. The vector-wise quantization uses separate normalization constants for each inner product in the matrix multiplication, resulting in improved quantization precision for most features. However, for the emergent outliers, the mixed-precision decomposition isolates the outlier feature dimensions into a 16-bit matrix multiplication while maintaining 8-bit multiplication for the remaining dimensions.

The authors provide empirical evidence that LLM.int8() enables the inference of LLMs with up to 175B parameters without any performance degradation. They show that regular quantization methods fail to maintain performance once systematic outliers occur in transformer layers. These outliers exhibit extreme magnitudes and negatively impact attention softmax probability mass and validation perplexity. LLM.int8() effectively deals with these outliers, preserving model performance.

The paper also discusses the interpretation of quantization performance, related work, and the limitations of the proposed method. The authors note that their analysis is focused on the Int8 data type and did not consider 8-bit floating-point (FP8) data types, as they are not currently supported by GPUs or TPUs. Additionally, the study only focuses on inference and does not explore training or finetuning

Words: 326