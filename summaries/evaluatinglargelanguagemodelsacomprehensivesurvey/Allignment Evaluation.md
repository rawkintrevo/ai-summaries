---
layout: page
title: Allignment Evaluation
date: 2023-11-30 21:35:45
---

[Back](./)


The content provided discusses the evaluation of language models (LLMs) on various criteria, including bias, toxicity, and truthfulness. The authors highlight different evaluation methods and datasets that have been developed to assess these criteria.

In terms of bias evaluation, the authors mention the Multilingual Holistic Bias dataset, which extends the HolisticBias dataset to 50 languages. This dataset evaluates biases in LLMs by providing models with ambiguous and disambiguous contexts and asking them to choose between options with and without stereotypes. Another dataset, BBQ, expands on this approach by including nine categories of biases and providing statistical bias scores to evaluate multiple question answering models. CBBQ extends BBQ to Chinese and includes additional categories based on Chinese socio-cultural factors. The authors also mention the need to use advanced LLMs or models trained on bias detection tasks for scoring bias and identifying biases in data for pre-training LLMs.

Next, the authors discuss the evaluation of toxicity in LLMs. They mention datasets such as OLID and SOLID for evaluating toxicity classification in English, as well as OLID-BR and KODOLI for evaluating toxicity in Brazilian Portuguese and Korean, respectively. They also highlight studies that have investigated LLMs' capability to detect and classify toxic content, both in English and non-English languages. The authors also mention the evaluation of toxicity in generated sentences using datasets like RealToxicityPrompts and HarmfulQ, as well as tools like PerspectiveAPI for measuring toxicity scores.

The authors then move on to the evaluation of truthfulness in LLMs. They mention several benchmark datasets that have been curated to assess truthfulness, including question answering datasets like NewsQA, SQuAD 2.0, BIG-bench, and SelfAware, dialogue datasets like DIALFACT, FactCC, and BEGIN, and summarization datasets like XSumFaith, FactCC, and AGGREFACT. They also discuss different methods for evaluating truthfulness, including NLI-based methods, QAQG-based methods, and LLM-based methods. NLI-based methods involve assessing the logical relationship between two pieces of text, while QAQG-based methods use question answering and question generation models to assess the factual consistency between generated text and source documents. LLM-based methods leverage the capability of LLMs to evaluate text quality and factuality.

Overall, the content provides a comprehensive overview of different evaluation methods and datasets for assessing bias, toxicity, and truthfulness in LLMs. It highlights the importance of evaluating these criteria to ensure the reliability and trustworthiness of LLM-generated content, particularly in applications such as finance, law, and medicine.

Words: 392