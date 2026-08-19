---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

### One2Three [IMWUT'26]

<p>    
<img  src="/images/One2Three.png"  width="350"  align="left" />
In recent years, Non-Line-of-Sight (NLoS) 3D object reconstruction has attracted enormous attention. Traditional approaches, while becoming increasingly accurate, rely on time-consuming two-dimensional (2D) scanning. This paper presents One2Three, an efficient 3D object reconstruction system with only one-dimensional (1D) scanning. One2Three proposes two mechanisms, Aliasing Signal Decoupling (ASD) and Simulated Multi-Size Synthetic Aperture Radar (SMS-SAR). Since the RF signal is highly affected by unknown yet prevalent environmental factors, leading to non-negligible inconsistencies across different scenes for the same object, we propose an Aliasing Signal Decoupling (ASD) mechanism that decouples the entangled signals of the target object and background reflections by analyzing the spatial-temporal correlations between the RF signals and the depth images. Then, we feed the pure object RF signals into our SMS-SAR module, which designs a multi-layer multi-scale convolution block to simulate a multi-resolution Synthetic Aperture Radar to learn the reconstruction principles.  
We conduct comprehensive experiments with 102 objects in 21 different environments. The results show that One2Three achieves comparable performance with the state-of-the-art 2D scanning approaches while reducing the time cost by $50\times\sim 200\times$ under the same scanning speed. One2Three also works well under complex situations, such as untrained objects, unseen environments, \etc. Our code and datasets will be released with this paper. 
</p>
- [Code](https://github.com/gdzchensir200127/One2Three)

### RF-Carer [SenSys'26]

<p>    
<img  src="/images/RF-carer.png"  width="350"  align="left" />
Respiratory monitoring using wireless technologies has garnered significant attention for its potential in healthcare, smart cockpits, and various applications. Though extensively studied, existing systems face practical challenges in adapting to new data domains without substantial customization efforts. Current solutions attempt to address this limitation through domain-independent feature extraction or cross-domain feature translation, employing either knowledge-based sensing models or data-driven neural networks. However, these approaches typically require additional data collection or model retraining for new domains, significantly hindering their practical deployment. This project introduces RF-Carer, a fully zero-effort cross-domain respiration monitoring system. 
Our key innovation lies in building an explainable propagation model to transform any heterogeneous signals under unknown domains into a unified form in the signal processing layer. 
To further address accidental irrelevant factors, we propose to align the feature spaces while suppressing the noisy ones with contrastive learning. 
On this basis, we develop a one-fits-all model. 
To the best of our knowledge, RF-Carer is the first zero-effort cross-domain respiration monitoring work with wireless RF signals and would be a fundamental step toward real-world deployments.
</p>
- [Code](https://github.com/GeWangXJTU/RF-Carer)
- [Dataset](https://drive.google.com/drive/folders/1fX-nAjrjg7fBlwBQtSeDgTav1de6OnMJ?usp=sharing)

### XRF V2 [IMWUT'25]

<p>    
<img  src="/images/xrfv2.png"  width="350"  align="left" />
  
Human action recognition usually assigns a label to a short, isolated action. XRF V2 moves toward a richer smart-home setting: a person performs continuous daily routines, the system localizes each action with start and end times, and those action tuples can be passed to an LLM agent to summarize behavior, answer task-oriented questions, or support home and health assistants.
The dataset integrates Wi-Fi CSI, IMU streams from consumer devices, and synchronized RGB-D-IR video. It was collected from 16 volunteers across three indoor environments: dining room, study room, and bedroom. After filtering incomplete recordings, XRF V2 contains 853 valid multimodal sequences and 16 h 16 min 8 s of data.
</p>
- [Website](https://aiotgroup.github.io/labpages/papers/xrf-v2-a-dataset-for-action-summarization-with-wi-fi-signals-and-imus-in-phones-watches-earbuds-and-glasses/index.html)
- [Code and Dataset](https://github.com/aiotgroup/XRFV2)
