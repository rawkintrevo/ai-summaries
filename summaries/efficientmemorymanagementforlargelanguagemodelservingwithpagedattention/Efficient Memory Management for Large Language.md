---
layout: page
title: Efficient Memory Management for Large Language
date: 2023-10-30 16:41:01
---
This paper introduces vLLM, a high-throughput serving system for large language models (LLMs) that efficiently manages memory using virtual memory and paging techniques. The system leverages a new attention algorithm called PagedAttention, which allows attention keys and values to be stored in non-contiguous paged memory. vLLM utilizes a block-oriented memory management scheme to ensure efficient memory usage, handle dynamic token lengths, and support different decoding algorithms.

vLLM addresses the memory limitations of LLM serving by dynamically allocating memory for the key-value (KV) cache of each request. It uses a mapping layer to translate logical blocks to physical blocks in memory, enabling efficient sharing and management of the KV cache. The system also implements a copy-on-write mechanism to handle modifications to shared blocks, reducing memory duplication and optimizing memory usage.

The paper presents several experiments to evaluate the performance of vLLM. The results show that vLLM outperforms existing LLM serving systems in terms of throughput and latency. The system can handle various decoding algorithms, such as parallel sampling and beam search, while efficiently managing memory.

The paper also discusses the impact of block size on vLLM's performance and compares the overhead of memory swapping and recomputation. It shows that smaller block sizes are more efficient for recomputation, while larger block sizes are more efficient for swapping.

Overall, vLLM provides a novel approach to efficiently managing memory in LLM serving, addressing the challenges posed by the memory limitations of large models. The system's virtual memory and paging techniques, along with its block-oriented memory management scheme, enable high-throughput serving of LLMs while optimizing memory usage.

Words: 262