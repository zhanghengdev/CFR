# Multispectral Fusion for Object Detection with Cyclic Fuse-and-Refine Blocks

By Heng Zhang, Elisa FROMONT, Sébastien LEFEVRE, Bruno AVIGNON

## Introduction

<img align="center" src="https://github.com/zhangheng19931123/CFR/blob/master/doc/cfr.png">

Multispectral images (e.g. visible and infrared) may be particularly useful when detecting objects with the same model in different environments (e.g. day/night outdoor scenes). To effectively use the different spectra, the main technical problem resides in the information fusion process. In this paper, we propose a new halfway feature fusion method for neural networks that leverages the complementary/consistency balance existing in multispectral features by adding to the network architecture, a particular module that cyclically fuses and refines each spectral feature. We evaluate the effectiveness of our fusion method on two challenging multispectral datasets for object detection. Our results show that implementing our Cyclic Fuse-and-Refine module in any network improves the performance on both datasets compared to other state-of-the-art multispectral object detection methods. 
For more details, please refer to our [ICIP paper](https://arxiv.org/pdf/2009.12664.pdf). 

## Results

In this repository we provide the detection results of CFR model for [KAIST dataset](https://soonminhwang.github.io/rgbt-ped-detection/). 

| **Reasonable-aLL** | **Reasonable-day** | **Reasonable-night** | **Runtime(1080Ti)** |
|:-----:|:-------:|:-------:|:-------:|
| 5.96% | 7.77% | 2.4% | 50ms | [Google Drive]


Note that the result reported in the paper was the averaged performance after repeating the experiments for ten times. The provided result belongs to one of the ten models. It is very close but slightly better than the averaged performance reported in the paper.

## Citing CFR

Please cite our paper in your publications if it helps your research:

    @InProceedings{ZHANG_2020_ICIP,
        TITLE = {Multispectral Fusion for Object Detection with Cyclic Fuse-and-Refine Blocks},
        AUTHOR = {Zhang, Heng and Fromont, Elisa and Lef{\`e}vre, S{\'e}bastien and Avignon, Bruno},
        URL = {https://hal.archives-ouvertes.fr/hal-02872132},
        BOOK
        TITLE = {ICIP 2020 - IEEE International Conference on Image Processing},
        ADDRESS = {Abou Dabi, United Arab Emirates},
        PAGES = {1-5},
        YEAR = {2020},
        MONTH = Oct, KEYWORDS = {Multispectral object detection ; Deep learning ; Multi- spectral feature fusion},
        PDF = {https://hal.archives-ouvertes.fr/hal-02872132/file/icip2020.pdf},
        HAL_ID = {hal-02872132},
        HAL_VERSION = {v1},
    } 