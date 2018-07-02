---
title: "Deep Sequence Learning with Auxiliary Information for Traffic Prediction"
collection: publications
permalink: /publication/2018-KDD-Traffic
date: 2018-08-19
venue: 'Proceedings of the 24th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining'
paperurl: 'https://arxiv.org/abs/1806.07380'
citation: 'Liao, Binbing, <b>Jingqing Zhang</b>, Chao Wu, Douglas McIlwraith, Tong Chen, Shengwen Yang, Yike Guo, and Fei Wu. "Deep Sequence Learning with Auxiliary Information for Traffic Prediction." In Proceedings of the 24th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining, ACM, 2018.'
authors: 'Binbing Liao, <b>Jingqing Zhang</b>, Chao Wu, Douglas McIlwraith, Tong Chen, Shengwen Yang, Yike Guo, Fei Wu'
---

###### Binbing Liao and Jingqing Zhang contributed equally to this article. 

[Download paper here](https://arxiv.org/pdf/1806.07380.pdf)

[Code and more info on GitHub](https://github.com/JingqingZ/BaiduTraffic)

## Abstract
Predicting traffic conditions from online route queries is a challenging task as there are many complicated interactions over the roads and crowds involved. In this paper, we intend to improve traffic prediction by appropriate integration of three kinds of implicit but essential factors encoded in auxiliary information. We do this within an encoder-decoder sequence learning framework that integrates the following data: 1) offline geographical and social attributes. For example, the geographical structure of roads or public social events such as national celebrations; 2) road intersection information, i.e. in general, traffic congestion occurs at major junctions; 3) online crowd queries. For example, when many online queries issued for the same destination due to a public performance, the traffic around the destination will potentially become heavier at this location after a while. Qualitative and quantitative experiments on a real-world dataset from Baidu have demonstrated the effectiveness of our framework.


## Q-Traffic Dataset
This dataset is now available at Baidu Research Open-Access Dataset (BROAD).

Link: [https://ai.baidu.com/broad/introduction?dataset=traffic](https://ai.baidu.com/broad/introduction?dataset=traffic).


## Citation
```
@inproceedings{bbliaojqZhangKDD18deep,  
  title = {Deep Sequence Learning with Auxiliary Information for Traffic Prediction},  
  author = {Binbing Liao and Jingqing Zhang and Chao Wu and Douglas McIlwraith and Tong Chen and Shengwen Yang  and Yike Guo and Fei Wu},  
  booktitle = {Proceedings of the 24th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining},  
  year = {2018},  
  organization = {ACM}  
}  
```
