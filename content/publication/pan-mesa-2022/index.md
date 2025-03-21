---
title: 'Mesa: A Memory-saving Training Framework for Transformers'
authors:
- Zizheng Pan
- Peng Chen
- Haoyu He
- Jing Liu
- Jianfei Cai
- Bohan Zhuang
date: '2022-08-01'
publishDate: '2025-03-14T12:48:48.057990Z'
publication_types:
- manuscript
publication: '*arXiv*'
doi: 10.48550/arXiv.2111.11124
abstract: There has been an explosion of interest in designing high-performance Transformers.
  While Transformers have delivered significant performance improvements, training
  such networks is extremely memory intensive owing to storing all intermediate activations
  that are needed for gradient computation during backpropagation, especially for
  long sequences. To this end, we present Mesa, a memory-saving training framework
  for Transformers. Specifically, Mesa uses exact activations during forward pass
  while storing a low-precision version of activations to reduce memory consumption
  during training. The low-precision activations are then dequantized during back-propagation
  to compute gradients. Besides, to address the heterogeneous activation distributions
  in the multi-head self-attention layers, we propose a head-wise activation quantization
  strategy, which quantizes activations based on the statistics of each head to minimize
  the approximation error. To further boost training efficiency, we learn quantization
  parameters by running estimates. More importantly, by re-investing the saved memory
  in employing a larger batch size or scaling up model size, we may further improve
  the performance under constrained computational resources. Extensive experiments
  on ImageNet, CIFAR-100 and ADE20K demonstrate that Mesa can achieve flexible memory-savings
  (up to 50%) during training while achieving comparable or even better performance.
  Code is available at https://github.com/ziplab/Mesa.
links:
- name: URL
  url: http://arxiv.org/abs/2111.11124
---
