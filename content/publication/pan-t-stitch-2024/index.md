---
title: 'T-Stitch: Accelerating Sampling in Pre-Trained Diffusion Models with Trajectory
  Stitching'
authors:
- Zizheng Pan
- Bohan Zhuang
- De-An Huang
- Weili Nie
- Zhiding Yu
- Chaowei Xiao
- Jianfei Cai
- Anima Anandkumar
date: '2024-02-01'
publishDate: '2025-03-14T12:48:48.060835Z'
publication_types:
- manuscript
publication: '*arXiv*'
doi: 10.48550/arXiv.2402.14167
abstract: Sampling from diffusion probabilistic models (DPMs) is often expensive for
  high-quality image generation and typically requires many steps with a large model.
  In this paper, we introduce sampling Trajectory Stitching T-Stitch, a simple yet
  efficient technique to improve the sampling efficiency with little or no generation
  degradation. Instead of solely using a large DPM for the entire sampling trajectory,
  T-Stitch first leverages a smaller DPM in the initial steps as a cheap drop-in replacement
  of the larger DPM and switches to the larger DPM at a later stage. Our key insight
  is that different diffusion models learn similar encodings under the same training
  data distribution and smaller models are capable of generating good global structures
  in the early steps. Extensive experiments demonstrate that T-Stitch is training-free,
  generally applicable for different architectures, and complements most existing
  fast sampling techniques with flexible speed and quality trade-offs. On DiT-XL,
  for example, 40% of the early timesteps can be safely replaced with a 10x faster
  DiT-S without performance drop on class-conditional ImageNet generation. We further
  show that our method can also be used as a drop-in technique to not only accelerate
  the popular pretrained stable diffusion (SD) models but also improve the prompt
  alignment of stylized SD models from the public model zoo. Code is released at https://github.com/NVlabs/T-Stitch
links:
- name: URL
  url: http://arxiv.org/abs/2402.14167
---
