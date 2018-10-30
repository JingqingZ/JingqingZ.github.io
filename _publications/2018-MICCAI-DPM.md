---
title: "The Deep Poincare Map: A Novel Approach for Left Ventricle Segmentation"
collection: publications
permalink: /publication/2018-MICCAI-DPM
date: 2018-09-16
venue: 'MICCAI 2018, the 21st International Conference on Medical Image Computing and Computer Assisted Intervention'
paperurl: '#'
citation: 'Yuanhan Mo, Fangde Liu, Douglas McIlwraith, Guang Yang, <b>Jingqing Zhang</b>, Taigang He, and Yike Guo. "The Deep Poincare Map: A Novel Approach for Left Ventricle Segmentation". MICCAI 2018, The 21st International Conference on Medical Image Computing and Computer-Assisted Intervention. 2018.'
authors: 'Yuanhan Mo, Fangde Liu, Douglas McIlwraith, Guang Yang, <b>Jingqing Zhang</b>, Taigang He, and Yike Guo'
---

Paper Link: [PDF](/files/pdf/miccai-2018-poincare.pdf)

More information will be published soon.

You may find another paper about DPM helpful [here](/publication/2017-DPM).

## Abstract
Precise segmentation of the left ventricle (LV) within cardiac MRI images is a prerequisite for the quantitative measurement of heart function. However, this task is challenging due to the limited availability of labeled data and motion artifacts from cardiac imaging. In this work, we present an iterative segmentation algorithm for LV delineation. By coupling deep learning with a novel dynamic-based labeling scheme, we present a new methodology where a policy model is learned to guide an agent to travel over the the image, tracing out a boundary of the ROI -- using the magnitude difference of the Poincar\'e map as a stopping criterion. Our method is evaluated on two datasets, namely the Sunnybrook Cardiac Dataset (SCD) and data from the STACOM 2011 LV segmentation challenge. Our method outperforms the previous research on many metrics. In order to demonstrate the transferability of our method we present encouraging results over the STACOM 2011 data, when using a model trained on the SCD dataset.

## Citation
```
@inproceedings{mo2018deep,
  title={The Deep Poincar{\'e} Map: A Novel Approach for Left Ventricle Segmentation},
  author={Mo, Yuanhan and Liu, Fangde and McIlwraith, Douglas and Yang, Guang and Zhang, Jingqing and He, Taigang and Guo, Yike},
  booktitle={International Conference on Medical Image Computing and Computer-Assisted Intervention},
  pages={561--568},
  year={2018},
  organization={Springer}
}
```