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
##### UPFD ![](https://img.shields.io/badge/-SocialGraph-red) which mainly focus on social graph and use the graph-based methods.
* Link to publication: [https://arxiv.org/pdf/2104.12259.pdf](https://arxiv.org/pdf/2104.12259.pdf)
* Link to data: [https://github.com/safe-graph/GNN-FakeNews](https://github.com/safe-graph/GNN-FakeNews)
* Task description: binary(fake,not)
* Details of task: graph-structured
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

#### Chinese
##### competition: BAAI & ICT - False news Detection ! [](https://img.shields.io/badge/-competition-orange)
* Link to competition: [https://www.biendata.xyz/competition/falsenews/](https://www.biendata.xyz/competition/falsenews/)
* Link to data: [https://www.biendata.xyz/competition/falsenews/data/](https://www.biendata.xyz/competition/falsenews/data/)
* Task description: binary(fake,not)
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


### Papers

#### Survey

#### Research Papers

### Organizations

### Contribution
