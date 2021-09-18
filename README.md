# Awesome Sign Language Rcognition and Sign Language Translation
<img src="img/sign_85_256.gif" width = "300">

A collection of resources about Sign Language Recognition (SLR) and Translation (SLT)

## Why awesome sign language recognition?
This is a collection of papers and resources I curated when learning the ropes in Sign Language Recognition and Translation. It is under construction and I will update it continuously. Feel free to contribute.

## Contributing
If you think I have missed out on something (or) have any suggestions (papers, implementations and other resources), feel free to [pull a request](https://github.com/jackyjsy/awesome-sign-language-estimation/pulls).

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
https://en.wikipedia.org/wiki/Sign_language    
https://towardsdatascience.com/sign-language-recognition-using-deep-learning-6549268c60bd
## Datasets
- [AUTSL](https://chalearnlap.cvc.uab.cat/dataset/40/description/) [[paper]](https://arxiv.org/abs/2008.00932)
- [SLR500 / SLR100](http://home.ustc.edu.cn/~pjh/openresources/cslr-dataset-2015/index.html)
- [WLASL](https://dxli94.github.io/WLASL/) [[paper]](https://arxiv.org/abs/1910.11006)
- [MS-ASL](https://www.microsoft.com/en-us/research/project/ms-asl/)
- [BSL-1K](https://www.robots.ox.ac.uk/~vgg/research/bsl1k/) [[paper]](https://arxiv.org/abs/2007.12131)

| Dataset  | Sign Language | # Classes | # Signers | # Samples | Type | Modalities | Year | Available * |
| ------------- | :-----------: | -: | -: | -: | :-: | :-: | :-: | :-: | 
| SLR500 isol.  | Chinese   | 500 | 50 | 125,000 | Isolated | RGB+D | 2016 | Yes |
| AUTSL   | Turkish   | 226 | 43 | 38,336 | Isolated | RGB+D | 2020 | Yes |
| WLASL   | American  | 2,000 | 119 | 21,083 | Isolated | RGB | 2020 | Yes |
| MS-ASL  | American  | 1,000 | 222 | 25,513 | Isolated | RGB | 2019 | No |
| BSL-1K  | British   | 1,064| 40 | 273,000 | Isolated | RGB | 2021 | No |
| SLR100 cont.     | Chinese   | 100 | 50 | 25,000 | Continuous | RGB+D | 2016 | Yes |

\* Availability at the moment.

## Papers

### Isolated sign language recognition
- [2021 CVPRW] Skeleton Aware Multi-modal Sign Language Recognition.[[paper]](https://openaccess.thecvf.com/content/CVPR2021W/ChaLearn/papers/Jiang_Skeleton_Aware_Multi-Modal_Sign_Language_Recognition_CVPRW_2021_paper.pdf)[[code]](https://github.com/jackyjsy/CVPR21Chal-SLR/)  
  *Songyao Jiang, Bin Sun, Lichen Wang, Yue Bai, Kunpeng Li, Yun Fu*
- [2021 TMM] Spatial-Temporal Multi-Cue Network for Sign Language Recognition and Translation.[[paper]](https://ieeexplore.ieee.org/abstract/document/9354538/)    
  *Hao Zhou, Wengang Zhou, Yun Zhou, Houqiang Li*
- [2021 AAAI] Hand-Model-Aware Sign Language Recognition.[[paper]](https://ojs.aaai.org/index.php/AAAI/article/view/16247)    
  *Hezhen Hu, Wengang Zhou, Houqiang Li*
- [2020 ECCV] BSL-1K: Scaling Up Co-articulated Sign Language Recognition Using Mouthing Cues.[[paper]](https://arxiv.org/abs/2007.12131)[[code]](https://github.com/gulvarol/bsl1k)   
  *Samuel Albanie, Gül Varol, Liliane Momeni, Triantafyllos Afouras, Joon Son Chung, Neil Fox, Andrew Zisserman*
### Continuous sign language recognition


### Sign language translation
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