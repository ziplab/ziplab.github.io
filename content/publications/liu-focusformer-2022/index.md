---
title: 'FocusFormer: Focusing on What We Need via Architecture Sampler'
authors:
- Jing Liu
- Jianfei Cai
- Bohan Zhuang
date: '2022-08-01'
publishDate: '2025-03-14T12:48:48.071537Z'
publication_types:
- manuscript
publication: '*arXiv*'
doi: 10.48550/arXiv.2208.10861
abstract: Vision Transformers (ViTs) have underpinned the recent breakthroughs in
  computer vision. However, designing the architectures of ViTs is laborious and heavily
  relies on expert knowledge. To automate the design process and incorporate deployment
  flexibility, one-shot neural architecture search decouples the supernet training
  and architecture specialization for diverse deployment scenarios. To cope with an
  enormous number of sub-networks in the supernet, existing methods treat all architectures
  equally important and randomly sample some of them in each update step during training.
  During architecture search, these methods focus on finding architectures on the
  Pareto frontier of performance and resource consumption, which forms a gap between
  training and deployment. In this paper, we devise a simple yet effective method,
  called FocusFormer, to bridge such a gap. To this end, we propose to learn an architecture
  sampler to assign higher sampling probabilities to those architectures on the Pareto
  frontier under different resource constraints during supernet training, making them
  sufficiently optimized and hence improving their performance. During specialization,
  we can directly use the well-trained architecture sampler to obtain accurate architectures
  satisfying the given resource constraint, which significantly improves the search
  efficiency. Extensive experiments on CIFAR-100 and ImageNet show that our FocusFormer
  is able to improve the performance of the searched architectures while significantly
  reducing the search cost. For example, on ImageNet, our FocusFormer-Ti with 1.4G
  FLOPs outperforms AutoFormer-Ti by 0.5% in terms of the Top-1 accuracy.
links:
- name: URL
  url: http://arxiv.org/abs/2208.10861
---
