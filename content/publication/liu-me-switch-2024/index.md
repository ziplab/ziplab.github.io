---
title: 'ME-Switch: A Memory-Efficient Expert Switching Framework for Large Language
  Models'
authors:
- Jing Liu
- Ruihao Gong
- Mingyang Zhang
- Yefei He
- Jianfei Cai
- Bohan Zhuang
date: '2024-10-01'
publishDate: '2025-03-14T12:48:48.077419Z'
publication_types:
- manuscript
publication: '*arXiv*'
doi: 10.48550/arXiv.2406.09041
abstract: LLM development involves pre-training a foundation model on massive data,
  followed by fine-tuning on task-specific data to create specialized experts. Serving
  these experts can pose significant memory challenges, as loading all experts onto
  devices is impractical, and frequent switching between experts in response to user
  requests can incur substantial I/O costs. Previous approaches decompose the expert
  weights as the pre-trained weights plus delta weights, followed by quantizing the
  delta weights using output channel-wise step sizes to reduce the model size. However,
  these methods overlook the fact that certain input channels of delta weights can
  cause significant quantization errors at extremely low bitwidths. Additionally,
  existing methods assume that the appropriate model for a user request is known in
  advance, which is not the case in practice. To this end, we introduce ME-Switch,
  a memory-efficient expert switching framework tailored for serving multiple LLMs.
  To condense the number of bits required for describing the delta weights, we propose
  a salient-aware delta compression method that identifies salient input channels
  based on reconstruction error and applies mixed-precision quantization, reducing
  non-salient channels to low bits while keeping salient ones intact, cutting storage
  demand without compromising performance. Moreover, we develop a model-level routing
  method that efficiently directs user queries to the most suitable expert by performing
  domain classification. Extensive experiments show the promising memory efficiency
  and routing performance of ME-Switch. For example, when serving three models from
  the Mistral-7B family, ME-Switch reduces the model size by $1.74times$ and maintains
  nearly lossless performance on instruction, mathematical reasoning, and code generation
  tasks. Notably, our method can efficiently serve 16 Mistral-7B models on a single
  NVIDIA A100 GPU.
links:
- name: URL
  url: http://arxiv.org/abs/2406.09041
---
