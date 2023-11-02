---
layout: page
title: ConvNets Match Vision Transformers at Scale
date: 2023-11-02 14:26:49
---
The paper titled "ConvNets Match Vision Transformers at Scale" by Samuel L Smith, Andrew Brock, Leonard Berrada, and Soham De from Google DeepMind challenges the belief that Convolutional Neural Networks (ConvNets) are not competitive with Vision Transformers (ViTs) on large datasets. The authors evaluate the performance of ConvNets pre-trained on a large labeled dataset called JFT-4B and compare it to ViTs with similar compute budgets.

The paper begins by providing background information on the success of ConvNets in computer vision and the recent rise of ViTs. The authors note that the computer vision community has shifted towards evaluating models pre-trained on large general-purpose datasets collected from the web. The question arises whether ViTs outperform ConvNets pre-trained with similar computational budgets.

To evaluate the scaling properties of ConvNets, the authors use the NFNet model family, which is a convolutional architecture that has previously set a new state-of-the-art (SOTA) on the ImageNet benchmark. They pre-train a range of NFNet models of varying depth and width on the JFT-4B dataset, which contains approximately 4 billion labeled images from 30,000 classes.

The authors observe a log-log scaling law between the validation loss and the compute budget used to pre-train the models. They find that as the compute budget increases, both the model size and the number of training epochs increase to achieve the lowest validation loss. The optimal learning rate for the models also decreases as the epoch budget increases.

After pre-training on JFT-4B, the authors fine-tune the pre-trained models on the ImageNet dataset. They use a technique called sharpness aware minimization (SAM) with stochastic depth and dropout for fine-tuning. The authors find that the ImageNet Top-1 accuracy consistently improves as the compute budget increases, reaching a maximum of 90.4% for their largest model.

Comparisons are made to pre-trained ViTs on ImageNet, and the authors find that their pre-trained NFNets achieve comparable performance with comparable compute budgets. They note that the performance of pre-trained NFNets at scale is remarkably similar to that of pre-trained ViTs. While ViTs have been pre-trained on much larger compute budgets, the authors estimate the pre-training efficiency of ViTs and NFNets on the same hardware and compare them.

The authors conclude that the most important factors determining the performance of a model are the compute and data available for training. They argue that there is no strong evidence to suggest that pre-trained ViTs outperform pre-trained ConvNets when evaluated fairly. However, they note that ViTs may have practical advantages in specific contexts, such as using similar model components across multiple modalities.

In summary, the paper challenges the belief that ConvNets are not competitive with ViTs on large datasets by demonstrating that pre-trained ConvNets, specifically NFNets, can achieve comparable performance with similar compute budgets. The authors highlight the importance of compute and data availability in determining model performance and provide evidence to support their findings.

Words: 473