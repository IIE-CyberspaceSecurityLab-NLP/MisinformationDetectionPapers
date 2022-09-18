# MisinformationDetectionPapers
Important papers on misinformation detection

## Contents

- [MisinformationDetectionPapers](#MisinformationDetectionPapers)
  - [Introduction](#introduction)
    - [Overview and Statistics](#statistics)
    - [Keywords Convention](#keywords-convention)
  - [Toolkits](#toolkits)
  - [Datasets](#datasets)
    - [English Datasets](#English)
    - [Chinese Datasets](#Chinese)
  - [Papers](#papers)
    - [Survey](#survey)
    - [Research Papers](#research-papers)
  - [Organizations](#organizations)
  - [Contribution](#contribution)


## Introduction

### Overview and Statistics

### Keywords Convention

<!-- ![](https://img.shields.io/badge/-UserInfo-green) which mainly focus on user info features. -->

![](https://img.shields.io/badge/-Text-blue) which mainly focus on the text features.

![](https://img.shields.io/badge/-Image-yellow) which means the dataset contains image datas

![](https://img.shields.io/badge/-SocialGraph-red) which mainly focus on social graph and use the graph-based methods.

![](https://img.shields.io/badge/-competition-orange) which means this dataset is from competition
<!-- ![](https://img.shields.io/badge/-Temporal-orange) which mainly focus on temporal patterns. -->

![](https://img.shields.io/badge/Conference-CCF--A-red) Conference Rank (A, B, C) from China Computer Federation.

### Toolkits

### Datasets

#### English
##### UPFD ![](https://img.shields.io/badge/-SocialGraph-red) 
* Link to publication: [https://arxiv.org/pdf/2104.12259.pdf](https://arxiv.org/pdf/2104.12259.pdf)
* Link to data: [https://github.com/safe-graph/GNN-FakeNews](https://github.com/safe-graph/GNN-FakeNews)
* Task description: binary(fake, not)
* Size of dataset: 5778
* Percentage fake: 50%
* Language: English
* Level of annotation: fake data obtained through Politifact and Gossipcop platforms
* Platform: Twitter
* Medium: text
* Citations: 32+
* Feature: 
    * id - Unique identifider for each news
    * url - Url of the article from web that published that news
    * title - Title of the news article
    * tweet_ids - Tweet ids of tweets sharing the news. This field is list of tweet ids separated by tab.
    * time - UNIX timestamp
* effect: 
    * Politifact: 
        * Acc: 84.62%(BERT)
        * F1: 84.53%(BERT)
    * Gossipcop:
        * Acc: 97.23%(BERT)
        * F1: 97.22%(BERT)
* Reference: Dou, Y., Shu, K., Xia, C., Yu, P. S., & Sun, L. (2021, July). User preference-aware fake news detection. In Proceedings of the 44th International ACM SIGIR Conference on Research and Development in Information Retrieval (pp. 2051-2055).

##### EANN-KDD18  ![](https://img.shields.io/badge/-Image-yellow)
* Link to publication: [https://dl.acm.org/citation.cfm?id=3219819.3219903](https://dl.acm.org/citation.cfm?id=3219819.3219903)
* Link to data: [https://github.com/yaqingwang/EANN-KDD18](https://github.com/yaqingwang/EANN-KDD18)
* Task description: binary(fake, not)
* Size of dataset: 
    * Twitter: 13924(514 tweets contain images)
    * Weibo: 9528(all contain images)
* Percentage fake: 
    * Twitter: 56.7%
    * Weibo: 49.8%
* Language: English, Chinese
* Level of annotation: 
    * Twitter: Multimodal data set from MediaEval, this dataset contains image, video, and context, here the author deletes tweets without any pictures and text //TODO
    * Weibo: The real data is obtained through China's authoritative news website, and the fake news is crawled by crawlers from 2012.5 to 2016.1, and the news is obtained through official Weibo rumors. Low quality and duplicate images were removed during collection. Divide the dataset into training, validation and test sets with a ratio of 7:1:2
* Platform: Twitter, Weibo
* Medium: text, image
* Citations: 499+
* Feature: 
* effect: 
    * Twitter:
        * Acc: 71.5%(EANN)
        * precision: 82.2%(EANN)
        * recall: 63.8%(EANN)
        * F1:71.9%(EANN)
    * Weibo:
    
* Reference: 

#### Chinese
##### competition: BAAI & ICT - False news Detection  ![](https://img.shields.io/badge/-competition-orange)
* Link to competition: [https://www.biendata.xyz/competition/falsenews/](https://www.biendata.xyz/competition/falsenews/)
* Link to data: [https://www.biendata.xyz/competition/falsenews/data/](https://www.biendata.xyz/competition/falsenews/data/)
* Task description: binary(fake, not)
* Details of task:
    1. False News Text Detection: text information only
    2. False News Image Detection: image information only
    3. False News Multi-Modal Detection: contains pictures and text information
* Size of dataset:
    1. Task1: 38471
    2. Task2: 34096
    3. Task3: 38471(text), 34096(image)
* Percentage fake:
    1. Task1: 50.1%
    2. Task2: 40.0%
    3. Task3: 50.1%
* Language: Chinese
* Level of annotation: news and rumors(have be officially debunked)
* Medium: Text,image,Text&image
* Feature:
    * id
    * text

##### EANN-KDD20  ![](https://img.shields.io/badge/-Image-yellow)
* Link to publication: [https://arxiv.org/abs/1912.12520](https://arxiv.org/abs/1912.12520)
* Link to data: [https://github.com/yaqingwang/WeFEND-AAAI20](https://github.com/yaqingwang/WeFEND-AAAI20)
* Task description: binary(fake,not)
* Size of dataset: 
    * train: 13330
    * test: 11623
    * non-label: 67748
* Percentage fake: 
    * train: 20.6%
    * test: 12.8%
* Language: English, Chinese
* Level of annotation: 
* Platform: WeChat
* Medium: text, image
* Citations: 
* Feature: 
* effect: 
* Reference: 

#### weibo21
* Link to publication: [https://arxiv.org/abs/2201.00987v1](https://arxiv.org/abs/2201.00987v1)
* Task description: binary(fake,real)
* Size of fake news: 4488
* Size of real news: 4640
* Language: Chinese
* Platform: Weibo
* Medium: text
* Feature: ID，content, comments, timestamp, label, category
* effect:
    * F1: 0.9137(MDFEND)
* reference: Nan Q, Cao J, Zhu Y, et al. MDFEND: Multi-domain fake news detection[C]//Proceedings of the 30th ACM International Conference on Information & Knowledge Management. 2021: 3343-3347.
#### wechat fake news
* Link to publication: [https://arxiv.org/abs/1912.12520](https://arxiv.org/abs/1912.12520)
* Task description: triple(fake, real, unlabeled)
* Size of fake news: 2090
* Size of real news: 2090
* Language: Chinese
* Platform: Wechat
* Medium: text
* Feature:
  * Official Account Name	--The name of official account, news publisher
  * Title	--News Title 
  * News Url	--The url of news 
  * Image Url	--The url of cover image 
  * Report Content	--The reports from reader, split by ## 
  * label --label of news, 0 is real and 1 is fake
* effect:
    * Fake news F1: 0.810
    * Real news F1: 0.836
* reference: Wang Y, Yang W, Ma F, et al. Weak supervision for fake news detection via reinforcement learning[C]//Proceedings of the AAAI conference on artificial intelligence. 2020, 34(01): 516-523.
#### Weibo FakeNews From USTC
* Link to publication: [https://justc.ustc.edu.cn/article/doi/10.52396/JUSTC-2021-0215](https://justc.ustc.edu.cn/article/doi/10.52396/JUSTC-2021-0215)
* Task description: binary(fake, real)
* Size of fake news: 26320
* Size of real news: 35426
* Size of fake user: 24181
* Language: Chinese
* Platform: Weibo
* Medium: text
* effect:
    * LSTM F1: 0.869
    * CNN F1: 0.899
*reference: Chen X, Fang S, Mao Z, et al. A data-driven model for social media fake news detection[J]. JUSTC, 2022, 52(3): 7-1-7-9.
### Papers

#### Survey

#### Research Papers

### Organizations

### Contribution
