# Awesome Sign Language Rcognition and Sign Language Translation
<img src="img/sign_85_256.gif" width = "300">

A collection of resources about Sign Language Recognition (SLR) and Translation (SLT)

## Why awesome sign language recognition?
This is a collection of papers and resources I curated when learning the ropes in Sign Language Recognition and Translation. It is under construction and I will update it continuously. Feel free to contribute.

## Contributing
If you think I have missed out on something (or) have any suggestions (papers, implementations and other resources), feel free to [pull a request](https://github.com/jackyjsy/awesome-sign-language-recognition/pulls).

Feedback and contributions are welcome!

## Table of Contents
- [Basics](#basics)
- [Datasets](#datasets)
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
[WIKI: Sign Language](https://en.wikipedia.org/wiki/Sign_language)    
[Awesome Sign Language Resources](https://github.com/surdoparasurdo/awesome-sign-language)   
[Basic Sign Language Recognition](https://towardsdatascience.com/sign-language-recognition-using-deep-learning-6549268c60bd)
## Datasets
- [AUTSL](https://chalearnlap.cvc.uab.cat/dataset/40/description/) [[paper]](https://arxiv.org/abs/2008.00932)
- [SLR500 / SLR100](http://home.ustc.edu.cn/~pjh/openresources/cslr-dataset-2015/index.html)
- [WLASL](https://dxli94.github.io/WLASL/) [[paper]](https://arxiv.org/abs/1910.11006)
- [MS-ASL](https://www.microsoft.com/en-us/research/project/ms-asl/)
- [BSL-1K](https://www.robots.ox.ac.uk/~vgg/research/bsl1k/) [[paper]](https://arxiv.org/abs/2007.12131)
- [How2Sign](https://how2sign.github.io/) [[paper]](https://openaccess.thecvf.com/content/CVPR2021/html/Duarte_How2Sign_A_Large-Scale_Multimodal_Dataset_for_Continuous_American_Sign_Language_CVPR_2021_paper.html)

| Dataset  | Sign Language | Classes | Signers | Videos | Type | Modalities | Year | Avail. * |
| ------------- | :-----------: | -: | -: | -: | :-: | :-: | :-: | :-: | 
| SLR500  | Chinese   | 500 | 50 | 125,000 | Isolated | RGB+D | 2016 | Yes |
| AUTSL   | Turkish   | 226 | 43 | 38,336 | Isolated | RGB+D | 2020 | Yes |
| WLASL   | American  | 2,000 | 119 | 21,083 | Isolated | RGB | 2020 | Yes |
| MS-ASL  | American  | 1,000 | 222 | 25,513 | Isolated | RGB | 2019 | No |
| BSL-1K  | British   | 1,064| 40 | 273,000 | Isolated | RGB | 2021 | No |
| SLR100  | Chinese   | 100 | 50 | 25,000 | Continuous | RGB+D | 2016 | Yes |
| How2Sign  | American   | \*\* | 11 | 35,000 | Continuous | RGB+D | 2021 | Yes |

\* Public availability at the moment.   
\*\* Vocabulary size 16k.

A more complete list of dataset can be found at https://how2sign.github.io/related_datasets.html

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
- [ICCV 2021] Visual Alignment Constraint for Continuous Sign Language Recognition.[[paper]](https://arxiv.org/abs/2104.02330)[[code]](https://github.com/ycmin95/VAC_CSLR)   
  *Yuecong Min, Aiming Hao, Xiujuan Chai, and Xilin Chen*   
<!-- - [ICCV 2021] Self-Mutual Distillation Learning for Continuous Sign Language Recognition.
  *Aiming Hao, Yuecong Min, and Xilin Chen* -->

### Sign language translation
- [2021 CVPR] Improving Sign Language Translation With Monolingual Data by Sign Back-Translation. [[paper]](https://arxiv.org/abs/2105.12397)   
  *Hao Zhou, Wengang Zhou, Weizhen Qi, Junfu Pu, Houqiang Li*
- [2020 AAAI] Spatial-Temporal Multi-Cue Network for Sign Language Recognition and Translation. [[paper]](https://arxiv.org/abs/2002.03187)   
  *Hao Zhou, Wengang Zhou, Yun Zhou, Houqiang Li*

## Benchmarks
[Paper with code](https://paperswithcode.com/task/sign-language-recognition)

## Challenges
[CVPR 2021 Looking at People Large Scale Signer Independent Isolated SLR Challenge](https://chalearnlap.cvc.uab.cat/challenge/43/description/)[[RGB](https://competitions.codalab.org/competitions/27901)][[RGB+D](https://competitions.codalab.org/competitions/27902)]

## Workshops
[CVPR 2021 ChaLearn Looking at People Sign Language Recognition in the Wild Workshop](https://chalearnlap.cvc.uab.cat/workshop/42/description/)

## Popular implementations
https://github.com/jackyjsy/CVPR21Chal-SLR/    
https://github.com/0aqz0/SLR