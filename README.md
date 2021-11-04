# Awesome Sign Language Rcognition and Sign Language Translation
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

<img src="img/sign_85_256.gif" width = "300">

A collection of resources about Sign Language Recognition (SLR) and Translation (SLT)

## Why awesome sign language recognition?
This is a collection of papers and resources I curated when learning the ropes in Sign Language Recognition and Translation. It is under construction and I will update it continuously. Feel free to contribute.

## Contributing
If you think I have missed out on something (or) have any suggestions (papers, implementations and other resources), feel free to [pull a request](https://github.com/jackyjsy/awesome-sign-language-recognition/pulls).

Feedback and contributions are welcome!

## Table of Contents
- [Basics](#basics)
- [Datasets](#popular-datasets)
- [Papers](#papers)
  - [Isolated sign language recognition](#isolated-sign-language-recognition)
  - [Continuous sign language recognition](#Continous-sign-language-recognition)
  - [Sign language translation](#sign-language-translation)
- [Benchmarks](#Benchmarks)
- [Challenges](#Challenges)
- [Workshops](#workshops) 
- [Popular implementations](#popular-implementations)
  - [PyTorch](#pytorch)
  <!-- - [TensorFlow](#tensorflow) -->
  <!-- - [Torch](#Torch) -->
  <!-- - [Others](#others) -->
<!-- - [Blog posts](#blogposts) -->

## Basics
- [WIKI: Sign Language](https://en.wikipedia.org/wiki/Sign_language)    
- [Awesome Sign Language Resources](https://github.com/surdoparasurdo/awesome-sign-language)   
- [Basic Sign Language Recognition](https://towardsdatascience.com/sign-language-recognition-using-deep-learning-6549268c60bd)   
- [Sign Language Recognition, Generation, and Translation:
An Interdisciplinary Perspective](https://arxiv.org/abs/1908.08597)
## Popular Datasets
- [AUTSL](https://chalearnlap.cvc.uab.cat/dataset/40/description/) [[paper]](https://arxiv.org/abs/2008.00932)
- [ICSL(SLR500) / CCSL(SLR100)](http://home.ustc.edu.cn/~pjh/openresources/cslr-dataset-2015/index.html)
- [WLASL](https://dxli94.github.io/WLASL/) [[paper]](https://arxiv.org/abs/1910.11006)
- [MS-ASL](https://www.microsoft.com/en-us/research/project/ms-asl/)
- [BSL-1K](https://www.robots.ox.ac.uk/~vgg/research/bsl1k/) [[paper]](https://arxiv.org/abs/2007.12131)
- [How2Sign](https://how2sign.github.io/) [[paper]](https://openaccess.thecvf.com/content/CVPR2021/html/Duarte_How2Sign_A_Large-Scale_Multimodal_Dataset_for_Continuous_American_Sign_Language_CVPR_2021_paper.html)   
- [CSL-Daily](http://home.ustc.edu.cn/~zhouh156/dataset/csl-daily/) [[paper]](https://arxiv.org/abs/2105.12397)

| Dataset  | Sign Language | Classes | Signers | Videos | Type | Modalities | Year | Avail. * |
| ------------- | :-----------: | -: | -: | -: | :-: | :-: | :-: | :-: | 
| SLR500  | Chinese   | 500 | 50 | 125,000 | Isolated | RGB+D | 2016 | Yes |
| AUTSL   | Turkish   | 226 | 43 | 38,336 | Isolated | RGB+D | 2020 | Yes |
| WLASL   | American  | 2,000 | 119 | 21,083 | Isolated | RGB | 2020 | Yes |
| MS-ASL  | American  | 1,000 | 222 | 25,513 | Isolated | RGB | 2019 | No |
| BSL-1K  | British   | 1,064| 40 | 273,000 | Isolated | RGB | 2021 | No |
| SLR100  | Chinese   | 100 | 50 | 25,000 | Continuous | RGB+D | 2016 | Yes |
| How2Sign  | American   | \*\* | 11 | 35,000 | Continuous | RGB+D | 2021 | Yes |
| PHOENIX-2014T | German | 1,066 | 9 | 8,257 | Translation | RGB | 2014 | Yes |
| CSL-Daily | Chinese | 2000 | 10 | 20,654 | Translaion | RGB | 2021 |

\* Public availability at the moment.   
\*\* Vocabulary size 16k.

Above is a brief summary of popular sign language dataset. A more complete list of dataset can be found at https://how2sign.github.io/related_datasets.html

## Papers

### Isolated sign language recognition
- [2021 CVPRW] Skeleton Aware Multi-modal Sign Language Recognition.[[paper]](https://openaccess.thecvf.com/content/CVPR2021W/ChaLearn/papers/Jiang_Skeleton_Aware_Multi-Modal_Sign_Language_Recognition_CVPRW_2021_paper.pdf)[[code]](https://github.com/jackyjsy/CVPR21Chal-SLR/)  
  *Songyao Jiang, Bin Sun, Lichen Wang, Yue Bai, Kunpeng Li, Yun Fu*
- [2021 TMM] Spatial-Temporal Multi-Cue Network for Sign Language Recognition and Translation.[[paper]](https://ieeexplore.ieee.org/abstract/document/9354538/)    
  *Hao Zhou, Wengang Zhou, Yun Zhou, Houqiang Li*
- [2021 AAAI] Hand-Model-Aware Sign Language Recognition.[[paper]](https://ojs.aaai.org/index.php/AAAI/article/view/16247)    
  *Hezhen Hu, Wengang Zhou, Houqiang Li*   
- [WACV 2021] Hand Pose Guided 3D Pooling for Word-level Sign Language Recognition.[[paper]](https://openaccess.thecvf.com/content/WACV2021/papers/Hosain_Hand_Pose_Guided_3D_Pooling_for_Word-Level_Sign_Language_Recognition_WACV_2021_paper.pdf)   
  *Al Amin Hosain; Panneer Selvam Santhalingam; Parth Pathak; Huzefa Rangwala; Jana Kosecka*   
- [2020 ECCV] BSL-1K: Scaling Up Co-articulated Sign Language Recognition Using Mouthing Cues.[[paper]](https://arxiv.org/abs/2007.12131)[[code]](https://github.com/gulvarol/bsl1k)   
  *Samuel Albanie, Gül Varol, Liliane Momeni, Triantafyllos Afouras, Joon Son Chung, Neil Fox, Andrew Zisserman*
### Continuous sign language recognition
- [2021 ICCV] Visual Alignment Constraint for Continuous Sign Language Recognition.[[paper]](https://arxiv.org/abs/2104.02330)[[code]](https://github.com/ycmin95/VAC_CSLR)   
  *Yuecong Min, Aiming Hao, Xiujuan Chai, and Xilin Chen*  
- [2020 ECCV] Fully Convolutional Networks for Continuous Sign Language Recognition.[[paper]](https://arxiv.org/abs/2007.12402)  
  *Ka Leong Cheng, Zhaoyang Yang, Qifeng Chen, and Yu-
Wing Tai*

- [2020 AAAI] Spatial-Temporal Multi-Cue Network for Continuous Sign Language Recognition. [[paper]](https://arxiv.org/abs/2002.03187)   
  *Hao Zhou, Wengang Zhou, Yun Zhou, Houqiang Li*
- [2019 CVPR] Iterative Alignment Network for Continuous Sign Language Recognition. [[paper]](https://openaccess.thecvf.com/content_CVPR_2019/papers/Pu_Iterative_Alignment_Network_for_Continuous_Sign_Language_Recognition_CVPR_2019_paper.pdf)   
  *Junfu Pu Wengang Zhou Houqiang Li*
- [2018 AAAI] Video-based Sign Language Recognition without Temporal Segmentation.[[paper]](https://arxiv.org/abs/1801.10111)   
  *Jie Huang, Wengang Zhou, Qilin Zhang, Houqiang Li, Weiping Li*
<!-- - [ICCV 2021] Self-Mutual Distillation Learning for Continuous Sign Language Recognition.
  *Aiming Hao, Yuecong Min, and Xilin Chen* -->

### Sign language translation
- [2021 ACMMM] Skeleton-Aware Neural Sign Language Translation. [[paper]](https://dl.acm.org/doi/pdf/10.1145/3474085.3475577)[[code]](https://github.com/SignLanguageCode/SANet)  
  *Shiwei Gan, Yafeng Yin, Zhiwei Jiang, Lei Xie, Sanglu Lu*  
- [2021 CVPR] Improving Sign Language Translation With Monolingual Data by Sign Back-Translation. [[paper]](https://arxiv.org/abs/2105.12397)   
  *Hao Zhou, Wengang Zhou, Weizhen Qi, Junfu Pu, Houqiang Li*
- [2021 TMM] Spatial-Temporal Multi-Cue Network for Sign Language Recognition and Translation. [[paper]](https://ieeexplore.ieee.org/abstract/document/9354538/)   
  *Hao Zhou, Wengang Zhou, Yun Zhou, Houqiang Li*
- [2020 NeurIPS] TSPNet: Hierarchical Feature Learning via Temporal Semantic Pyramid for Sign Language Translation. [[paper]](https://arxiv.org/pdf/2010.05468v1.pdf)[[code]](https://github.com/verashira/TSPNet)   
  *Dongxu Li, Chenchen Xu, Xin Yu, Kaihao Zhang, Ben Swift, Hanna Suominen, Hongdong Li*
- [2018 CVPR] Neural Sign Language Translation [[paper]](https://openaccess.thecvf.com/content_cvpr_2018/papers/Camgoz_Neural_Sign_Language_CVPR_2018_paper.pdf)[[code]](https://github.com/neccam/nslt)   
  *Necati Cihan Camgoz, Simon Hadfield, Oscar Koller, Hermann Ney, Richard Bowden*
## Benchmarks
[Paper with code](https://paperswithcode.com/task/sign-language-recognition)

## Challenges
[CVPR 2021 Looking at People Large Scale Signer Independent Isolated SLR Challenge](https://chalearnlap.cvc.uab.cat/challenge/43/description/) [[RGB]](https://competitions.codalab.org/competitions/27901)[[RGB+D]](https://competitions.codalab.org/competitions/27902)[[paper]](https://openaccess.thecvf.com/content/CVPR2021W/ChaLearn/papers/Sincan_ChaLearn_LAP_Large_Scale_Signer_Independent_Isolated_Sign_Language_Recognition_CVPRW_2021_paper.pdf)

## Workshops
[CVPR 2021 ChaLearn Looking at People Sign Language Recognition in the Wild Workshop](https://chalearnlap.cvc.uab.cat/workshop/42/description/)

## Popular implementations
https://github.com/jackyjsy/CVPR21Chal-SLR/    
https://github.com/0aqz0/SLR