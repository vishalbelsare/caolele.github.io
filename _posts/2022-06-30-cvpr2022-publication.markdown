---
layout: post
title:  Two Papers Published in CVPR 2022 - Information Fusion in Transformer for Vision Tasks
date:   2022-06-30 23:15:30 +0300
image:  /assets/images/blog/cvpr2022.jpg
author: Lele Cao
tags:   Computer Vision Research
---

**I am super happy to share that two research work I participated got accepted and published by [CVPR 2022](https://cvpr2022.thecvf.com/).🎉** 

The Conference on Computer Vision and Pattern Recognition (CVPR) is an annual conference on computer vision and pattern recognition, which is regarded as one of the most important conferences in its field. According to [Google 2022 academic indicators](https://scholar.google.com/citations?view_op=top_venues), CVPR maintains the 4th place, second only to Science.

As a former Ph.D. Researcher in [Tsinghua University](https://www.tsinghua.edu.cn/en/), I feel humbled and trilled to be able to continue contributing to the important researches carried out there. Both papers are about information fusion using Transformer, the learning from which could be useful to my work in EQT.

☝🏻 In [the 1st work](https://openaccess.thecvf.com/content/CVPR2022/html/Wang_Multimodal_Token_Fusion_for_Vision_Transformers_CVPR_2022_paper.html), we propose an adaptive multimodal fusion method tailored for transformer-based vision tasks.

✌🏻 In [the 2nd work](https://openaccess.thecvf.com/content/CVPR2022/html/Wang_Bridged_Transformer_for_Vision_and_Point_Cloud_3D_Object_Detection_CVPR_2022_paper.html), we propose an e2e architecture for 3D object detection, which utilizes the object queries for bridging 3D and 2D spaces.


**Multimodal Token Fusion for Vision Transformers**

Many adaptations of transformers have emerged to address the single-modal vision tasks, where self-attention modules are stacked to handle input sources like images. Intuitively, feeding multiple modalities of data to vision transformers could improve the performance, yet the inner-modal attentive weights may be diluted, which could thus greatly undermine the final performance. In this paper, we propose a multimodal token fusion method (TokenFusion), tailored for transformer-based vision tasks. To effectively fuse multiple modalities, TokenFusion dynamically detects uninformative tokens and substitute these tokens with projected and aggregated inter-modal features. Residual positional alignment is also adopted to enable explicit utilization of the inter-modal alignments after fusion. The design of TokenFusion allows the transformer to learn correlations among multimodal features, while the single-modal transformer architecture remains largely intact. Extensive experiments are conducted on a variety of homogeneous and heterogeneous modalities and demonstrate that TokenFusion surpasses state-of-the-art methods in three typical vision tasks: multimodal image-to-image translation, RGB-depth semantic segmentation, and 3D object detection with point cloud and images.

Links: [paper](https://openaccess.thecvf.com/content/CVPR2022/papers/Wang_Multimodal_Token_Fusion_for_Vision_Transformers_CVPR_2022_paper.pdf), [appendix](https://openaccess.thecvf.com/content/CVPR2022/supplemental/Wang_Multimodal_Token_Fusion_CVPR_2022_supplemental.pdf), [bibtex](https://openaccess.thecvf.com/content/CVPR2022/html/Wang_Multimodal_Token_Fusion_for_Vision_Transformers_CVPR_2022_paper.html#:~:text=arXiv%5D%20%5B-,bibtex,-%5D)

**Bridged Transformer for Vision and Point Cloud 3D Object Detection**

3D object detection is a crucial research topic in computer vision, which usually uses 3D point clouds as input in conventional setups. Recently, there is a trend of leveraging multiple sources of input data, such as complementing the 3D point cloud with 2D images that often have richer color and fewer noises. However, due to the heterogeneous geometrics of the 2D and 3D representations, it prevents us from applying off-the-shelf neural networks to achieve multimodal fusion. To that end, we propose Bridged Transformer (BrT), an end-to-end architecture for 3D object detection. BrT is simple and effective, which learns to identify 3D and 2D object bounding boxes from both points and image patches. A key element of BrT lies in the utilization of object queries for bridging 3D and 2D spaces, which unifies different sources of data representations in Transformer. We adopt a form of feature aggregation realized by point-to-patch projections which further strengthen the interaction between images and points. Moreover, BrT works seamlessly for fusing the point cloud with multi-view images. We experimentally show that BrT surpasses state-of-the-art methods on SUN RGB-D and ScanNetV2 datasets.

Links: [pdf](https://openaccess.thecvf.com/content/CVPR2022/papers/Wang_Bridged_Transformer_for_Vision_and_Point_Cloud_3D_Object_Detection_CVPR_2022_paper.pdf), [supp](https://openaccess.thecvf.com/content/CVPR2022/supplemental/Wang_Bridged_Transformer_for_CVPR_2022_supplemental.pdf), [bibtex](https://openaccess.thecvf.com/content/CVPR2022/html/Wang_Bridged_Transformer_for_Vision_and_Point_Cloud_3D_Object_Detection_CVPR_2022_paper.html#:~:text=supp%5D%20%5B-,bibtex,-%5D)