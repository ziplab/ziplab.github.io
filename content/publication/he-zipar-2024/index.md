---
title: 'ZipAR: Accelerating Auto-regressive Image Generation through Spatial Locality'
authors:
- Yefei He
- Feng Chen
- Yuanyu He
- Shaoxuan He
- Hong Zhou
- Kaipeng Zhang
- Bohan Zhuang
date: '2024-12-01'
publishDate: '2025-03-14T12:48:48.080433Z'
publication_types:
- manuscript
publication: '*arXiv*'
doi: 10.48550/arXiv.2412.04062
abstract: "In this paper, we propose ZipAR, a training-free, plug-and-play parallel\
  \ decoding framework for accelerating auto-regressive (AR) visual generation. The\
  \ motivation stems from the observation that images exhibit local structures, and\
  \ spatially distant regions tend to have minimal interdependence. Given a partially\
  \ decoded set of visual tokens, in addition to the original next-token prediction\
  \ scheme in the row dimension, the tokens corresponding to spatially adjacent regions\
  \ in the column dimension can be decoded in parallel, enabling the ``next-set prediction''\
  \ paradigm. By decoding multiple tokens simultaneously in a single forward pass,\
  \ the number of forward passes required to generate an image is significantly reduced,\
  \ resulting in a substantial improvement in generation efficiency. Experiments demonstrate\
  \ that ZipAR can reduce the number of model forward passes by up to 91% on the Emu3-Gen\
  \ model without requiring any additional retraining. Code is available here: https://github.com/ThisisBillhe/ZipAR."
links:
- name: URL
  url: http://arxiv.org/abs/2412.04062
---
