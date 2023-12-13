---
layout: page
title: Purple Llama CYBERSECEVAL
date: 2023-12-13 17:21:19
---

[Back](./)


Large Language Models (LLMs) have become increasingly capable of generating functional code in response to natural language requests. However, there is a lack of research on measuring and mitigating cybersecurity risks associated with LLMs. In this paper, the authors introduce CYBERSECEVAL, a comprehensive cybersecurity safety measurement suite for LLMs. 

The authors identify two major cybersecurity risks posed by LLMs. First, LLMs may generate code that fails to follow security best practices or introduces vulnerabilities. Previous studies have shown that developers readily accept significant amounts of code suggested by LLMs, and a substantial proportion of these suggestions are found to be vulnerable. To mitigate this risk, CYBERSECEVAL employs the Insecure Code Detector (ICD), a knowledge base of static analysis rules designed to identify insecure coding practices. The ICD is used to generate test cases and evaluate LLM responses, helping to identify risks and provide directions for improvement.

The second cybersecurity risk identified is the possibility of LLMs assisting in malicious activities related to computer systems. The authors investigate whether LLMs align to resist helping in illicit activities when it comes to coding-enabled models. They highlight that the intent behind the code is crucial, as code alone is not inherently malicious or benign. CYBERSECEVAL evaluates the compliance of LLMs with requests to assist in cyberattacks, providing insights into potential misuse scenarios. By understanding how LLMs respond to such requests, developers can implement safety measures to prevent models from being misused.

CYBERSECEVAL's approach to measuring cybersecurity risks involves two main components: insecure coding practice testing and cyberattack helpfulness testing. In the insecure coding practice testing, the ICD is used to detect insecure coding practices in LLM output. Test cases are generated based on instances of insecure coding practices found in open source code, and LLM responses are evaluated to determine if they reproduce or avoid these insecure practices. The evaluation of cyberattack helpfulness involves creating test cases that prompt LLMs to assist in carrying out cyberattacks as defined by the MITRE ATT&CK® ontology. LLM responses are evaluated to determine if they are helpful in executing a cyberattack.

The authors present the main contributions of CYBERSECEVAL, including its breadth (covering multiple programming languages and cybersecurity weaknesses), realism (using real-world code scenarios), adaptability (easily adaptable to assess new weaknesses and attack tactics), and accuracy in evaluating LLM completions for cybersecurity safety.

The paper also includes a case study in which CYBERSECEVAL is applied to Llama 2, Code Llama, and OpenAI GPT LLMs. The study reveals that all models exhibit insecure coding practices to a significant degree, with higher coding ability models being more prone to suggesting insecure code. In terms of compliance with requests to help carry out cyberattacks, models exhibit varying rates of compliance, with higher coding ability models having a higher rate of compliance compared to non-code-specialized models.

The paper concludes by discussing related work in the field and highlighting the limitations of CYBERSECEVAL. The authors provide information on how to access and run CYBERSECEVAL using their open GitHub repository and emphasize the need for ongoing research and development to enhance the safety and security of LLMs.

Words: 514