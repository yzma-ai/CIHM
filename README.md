# CIHM

### Official PyTorch Implementation

> **Paper Title:** CIHM: Context-Insight Hybrid Mamba for Efficient Medical Image Segmentation  
> **Authors:** Ma YiZe et al.  

---

## 🚀 Introduction

**This repository contains the official source code for "CIHM".**

The code and pretrained models will be released **upon acceptance** of the paper. We are currently organizing the code and documentation to ensure reproducibility.

## 📌 Abstract

In medical image segmentation, U-Net and its variants are widely utilized. However, CNN-based models suffer from limitations in long-range dependency modeling, while transformer-based models are constrained by quadratic computational complexity. Recently, state space models (SSMs) such as Mamba have emerged as a promising solution, as they excel at modeling long-range interactions while maintaining linear computational complexity. 

This paper proposes the **CIHM**, a hybrid Mamba model that provides contextual insights. Its key component is the **Context-Insight Mamba-CNN layer (CiMC layer)**. The CiMC layer adopts a hybrid Mamba-CNN approach to process features across different scales and levels in parallel, thereby enhancing the semantic segmentation of medical images. Specifically, the SSM branch of this layer captures long-range dependencies with comprehensive contextual semantic understanding, while the CNN block achieves superior local feature extraction using T-shaped convolution that focuses on patch centers. Moreover, to further aggregate multi-scale contextual information of medical images, we design the **Multiscale Refining Detail Bridge (MRDB)** module. This module significantly improves feature representation through dense multiplication and concatenation of features for fusion. 

Comprehensive experiments on the **ISIC2017**, **ISIC2018**, **Synapse**, and **DSB18** datasets demonstrate that CIHM exhibits strong competitive performance and efficiency in medical image segmentation tasks. Notably, compared to the well-known U-Net and the modern hybrid network U-Mamba, CIHM achieves better segmentation performance while reducing the parameter count by **40x** and **345x**, respectively. This highlights the potential of our approach in advancing model lightweighting.

## 📅 TODO / Updates

- [x] Create the repository.
- [ ] Release the training and inference code (Coming Soon).
- [ ] Release the pretrained models.

## 📧 Contact

If you have any questions, please feel free to contact **Ma YiZe** at `yzma@m.fudan.edu.cn`.
