## Autonomous-Databases



# Table of Contents

* [0. Survey and Tutorial (16)](#0-survey-and-tutorial)
* [1. Database Configuration](#1-database-configuration)
  * [1.1 Knob Tuner (23)](#knob-tuner)
  * [1.2 View Advisor (9)](#view-advisor)
  * [1.3 Index Advisor (86)](#index-advisor)
  * [1.4 Partition Advisor (11)](#partition-advisor)
  * [1.5 Hybrid Advisor (2)](#hybrid-advisor)
* [2. Query Optimization](#2-query-optimization)
  * [2.1 Query Rewriter (13)](#query-rewriter)
  * [2.2 Cardinality Estimation (36)](#cardinality-estimation)
  * [2.3 Cost Estimation (3)](#cost-estimation)
  * [2.4 Plan Optimization (25)](#plan-optimization)
* [3. Workload Scheduling (2)](#3-workload-scheduling)
* [4. Database Design](#4-database-design)
  * [4.1 Learned Index (30)](#index)
  * [4.2 Learned Layout (6)](#layout)
  * [4.3 Query Execution (3)](#query-execution)
* [5. Database Monitoring (12)](#5-database-monitoring)
* [6. Database Diagnosis](#6-database-diagnosis)
  * [6.1 System Diagnosis (7)](#system-and-kernel-causes)
  * [6.2 Query Diagnosis (1)](#bottleneck-queries)
* [7. General Techniques](#7-general-techniques)
  * [7.1 Feature Engineering for DB (7)](#feature-engineering-for-db)
  * [7.2 Feature Engineering for AI (6)](#feature-engineering-for-ai)
  * [7.3 Model Transfer (2)](#model-transfer) 
  * [7.4 Query And Data Generation (5)](#query-and-data-generation)
* [8. Database Frameworks (18)](#8-database-frameworks)
* [9. Demonstrations (13)](#9-demonstrations)
* [S1. LLM x DB (33)](#s1-large-language-models-meet-database)
* [S2. AI Resources (5)](#s2-ai-paper-and-code-list)
* [S3. Data And SQLs (3)](#s3-open-datasets-and-sqls)

------

## 0. Survey and Tutorial

### Survey



### Tutorial

**Spatial Query Optimization With Learning**

Xin Zhang and Ahmed Eldawy. PVLDB, 17(12): 4245 - 4248, 2024.[[paper](https://www.vldb.org/pvldb/vol17/p4245-zhang.pdf)]

**Databases Unbound: Querying All of the World’s Bytes with AI**

Samuel Madden, Michael Cafarella, Michael Franklin, and Tim Kraska.  PVLDB, 17(12): 4546-4554, 2024.[[paper](https://www.vldb.org/pvldb/vol17/p4546-madden.pdf)]

**Learned Query Optimizer: What is New and What is Next**

Rong Zhu, Lianggui Weng, Bolin Ding, and Jingren Zhou. 2024.In Companion of the 2024 International Conference on Management of Data (SIGMOD-Companion ’24), June 9–15, 2024, Santiago, AA, Chile. ACM, New York, NY, USA, 9 pages.[[paper](https://dl.acm.org/doi/10.1145/3626246.3654692)]

**Machine Learning for Databases: Foundations, Paradigms, and Open problems**

Gao Cong, Jingyi Yang, and Yue Zhao. 2024. In Companion of the 2024 International Conference on Management of Data (SIGMOD-Companion ’24), June 9–15, 2024, Santiago, AA, Chile. ACM, New York, NY, USA, 8 pages.[[paper](https://dl.acm.org/doi/10.1145/3626246.3654686)]

## 1. Database Configuration

### Knob Tuner

#### Heuristic

**An Eficient Transfer Learning Based Configuration Adviser for Database Tuning**

Xinyi Zhang, Hong Wu, Yang Li, Zhengju Tang, Jian Tan, Feifei Li, and Bin Cui. PVLDB, 17(3): 539 - 552, 2023.[[paper](https://www.vldb.org/pvldb/vol17/p539-zhang.pdf)]

------



#### BO-based



------



#### DL-based



------



#### RL-based



------



#### Knob Selection

**Explainable Database Management System Configuration Tuning through Counterfactuals**

Xinyue Shao, Hongzhi Wang, Xiao Zhu, Tianyu Mu, Yan Zhang. ICDE, 2024. [[paper](https://ieeexplore.ieee.org/document/10597897)]

------



#### Benefit Estimation

**Can Uncertainty Quantification Enable Better Learning-based Index Tuning?**

Tao Yu, Zhaonian Zou, Hao Xiong. (2024). [[paper](https://arxiv.org/pdf/2410.17748)]

------



#### Experiments

**KnobCF: Uncertainty-aware Knob Tuning**

Yan Y, Huang J, Wang H, et al. arXiv preprint arXiv:2407.02803, 2024.[[paper](https://arxiv.org/abs/2407.02803)]

**Functionality-Aware Database Tuning via Multi-Task Learning**

Zhongwei Yue, Shujian Peng, Peng Cai, Xuan Zhou, Huiqi Hu, Rong Zhang, Quanqing Xu, Chuanhui Yang. ICDE, 2024. [[paper](https://ieeexplore.ieee.org/document/10598099)]

------



### View Advisor

### Index Advisor

#### Workload Compression

#### Offline Index Tuning

**LeaderKV: Improving Read Performance of KV Stores via Learned Index and Decoupled KV Table**

Yi Wang, Jianan Yuan, Shangyu Wu, Huan Liu, Jiaxian Chen, Chenlin Ma, Jianbin Qin. ICDE 2024. [[paper](https://ieeexplore.ieee.org/document/10597902)]

#### Online Index Tuning



#### Index Benefit Estimation



#### Adaptive Indexing

**Towards Systematic Index Dynamization**

Douglas B. Rumbaugh, Dong Xie, and Zhuoyue Zhao. PVLDB, 17(11): 2867 - 2879, 2024.[[paper](https://www.vldb.org/pvldb/vol17/p2867-rumbaugh.pdf)]

**Chameleon: Towards Update-Efficient Learned Indexing for Locally Skewed Data**

Na Guo, Yaqi Wang, Wenli Sun, Yu Gu,  Jianzhong Qi, Zhenghao Liu, Xiufeng Xia, Ge Yu. ICDE 2024. [[paper](https://ieeexplore.ieee.org/document/10597777)]

### Partition Advisor

### Hybrid Advisor

## 2. Query Optimization

### Query Rewriter

#### Traditional

**Window Function Expression: Let the Self-join Enter**

Radim Bača. PVLDB, 17(9): 2162 - 2174, 2024. [[paper](https://www.vldb.org/pvldb/vol17/p2162-baca.pdf)]

**Efficient Enumeration of Recursive Plans in Transformation-based Query Optimizers**

Amela Fejza, Pierre Genevès, and Nabil Layaïda. PVLDB, 17(11): 3095 - 3108, 2024. [[paper](https://www.vldb.org/pvldb/vol17/p3095-geneves.pdf)]

**Query Optimization by Quantifier Elimination**

Christoph Koch and Peter Lindner. SIGMOD 2024. [[paper](https://dl.acm.org/doi/10.1145/3651607)]

**Dias: Dynamic Rewriting of Pandas Code**

Stefanos Baziotis, Daniel Kang, and Charith Mendis. SIGMOD 2024. [[paper](https://dl.acm.org/doi/10.1145/3639313)]

#### Learning-based





### Cardinality Estimation

**UltraLogLog: A Practical and More Space-Efficient Alternative to HyperLogLog for Approximate Distinct Counting**

Otmar Ertl. PVLDB, 17(7): 1655 - 1668, 2024. [[paper](https://dl.acm.org/doi/10.14778/3654621.3654632)]

**Cardinality Estimation of Subgraph Matching: A Filtering-Sampling Approach**

Wonseok Shin, Siwoo Song, Kunsoo Park, and Wook-Shin Han. PVLDB, 17(7): 1697 - 1709, 2024. [[paper](https://dl.acm.org/doi/10.14778/3654621.3654635)]

**ByteCard: Enhancing ByteDance's Data Warehouse with Learned Cardinality Estimation**

Yuxing Han, Haoyu Wang, Lixiang Chen, Yifeng Dong, Xing Chen, Benquan Yu, Chengcheng Yang, and Weining Qian. SIGMOD 2024. [[paper](https://dl.acm.org/doi/abs/10.1145/3626246.3653376)]

**ASM in Action: Fast and Practical Learned Cardinality Estimation**

Sangoh Lee, Kyoungmin Kim, and Wook-Shin Han. SIGMOD 2024. [[paper](https://dl.acm.org/doi/10.1145/3626246.3654728)]

**ASM: Harmonizing Autoregressive Model, Sampling, and Multi-dimensional Statistics Merging for Cardinality Estimation**

Kyoungmin Kim, Sangoh Lee, Injung Kim, and Wook-Shin Han. 2024. [[paper](https://dl.acm.org/doi/10.1145/3639300)]

### Cost Estimation

**DACE: A Database-Agnostic Cost Estimator**

Zibo Liang, Xu Chen, Yuyang Xia, Runfan Ye, Haitian Chen, Jiandong Xie, Kai Zheng. ICDE 2024. [[paper](https://ieeexplore.ieee.org/document/10598079)]

**Costream: Learned Cost Models for Operator Placement in Edge-Cloud Environments**

R. Heinrich, C. Binnig, H. Kornmayer and M. Luthra. ICDE 2024. [[paper](https://ieeexplore.ieee.org/document/10598052)]

### Plan Optimization

**Towards Exploratory Query Optimization for Template-Based SQL Workloads**

J. Feng, Z. Li and Q. Chen. ICDE 2024. [[paper](https://ieeexplore.ieee.org/document/10597755)]

**FOSS: A Self-Learned Doctor for Query Optimizer**

K. Zhong, L. Sun, T. Ji, C. Li and H. Chen. ICDE 2024. [[paper](https://ieeexplore.ieee.org/document/10597900)]

**GLO: Towards Generalized Learned Query Optimization**

T. Chen, J. Gao, Y. Tu and M. Xu. ICDE 2024. [[paper](https://ieeexplore.ieee.org/document/10597975)]

## 3. Workload Scheduling

**Towards Optimal Transaction Scheduling**

Audrey Cheng, Aaron Kabcenell, Jason Chan, Xiao Shi, Peter Bailis, Natacha Crooks, Ion Stoica. PVLDB, 17(11): 2694 - 2707, 2024. [[paper](https://www.vldb.org/pvldb/vol17/p2694-cheng.pdf)]

**RobOpt: A Tool for Robust Workload Optimization Based on Uncertainty-Aware Machine Learning**

Amin Kamali, Verena Kantere, Calisto Zuzarte, and Vincent Corvinelli. SIGMOD 2024. [[paper](https://dl.acm.org/doi/10.1145/3626246.3654755)]

**Sibyl: Forecasting Time-Evolving Query Workloads**

Hanxian Huang, Tarique Siddiqui, Rana Alotaibi, Carlo Curino, Jyoti Leeka, Alekh Jindal, Jishen Zhao, Jesús Camacho-Rodríguez, and Yuanyuan Tian. SIGMOD 2024. [[paper](https://dl.acm.org/doi/10.1145/3639308)]

## 4. Database Design

### Index

#### One-dimensional Index



#### Multi-dimensional Index

#### Experiment and Analysis



### Layout

**Automated Multidimensional Data Layouts in Amazon Redshif**

Jialin Ding, Matt Abrams, Sanghita Bandyopadhyay, Luciano Di Palma, Yanzhu Ji, Davide Pagano, Gopal Paliwal, Panos Parchas, Pascal Pfeil, Orestis Polychroniou, Gaurav Saxena, Aamer Shah, Amina Voloder, Sherry Xiao, Davis Zhang, and Tim Kraska. SIGMOD 2024. [[paper](https://dl.acm.org/doi/10.1145/3626246.3653379)]

**Dynamic Data Layout Optimization with Worst-case Guarantees**

K. Rong, P. Liu, S. A. Sonje and M. Charikar. ICDE 2024. [[paper](https://ieeexplore.ieee.org/document/10597977)]

### Query Execution

**Hit the Gym: Accelerating Query Execution to Efficiently Bootstrap Behavior Models for Self-Driving Database Management Systems**

Wan Shen Lim, Lin Ma, William Zhang, Matthew Butrovich, Samuel Arch, and Andrew Pavlo. PVLDB, 17(11): 3680 - 3693, 2024. [[paper](https://www.vldb.org/pvldb/vol17/p3680-lim.pdf)]

**Optimizing Disjunctive Queries with Tagged Execution**

Albert Kim and Samuel Madden. SIGMOD 2024. [[paper](https://dl.acm.org/doi/10.1145/3654961)]

**LAQUE: Automated Predicate Learning at Query Time**

Yiming Lin and Sharad Mehrotra. SIGMOD 2024. [[paper](https://dl.acm.org/doi/10.1145/3639301)]

**ROME: Robust Query Optimization via Parallel Multi-Plan Execution**

Ziyun Wei and Immanuel Trummer. SIGMOD 2024. [[paper](https://dl.acm.org/doi/10.1145/3654973)]

## 5. Database Monitoring

**IsoVista: Black-box Checking Database Isolation Guarantees**

Long Gu, Si Liu, Tiancheng Xing, Hengfeng Wei, Yuxing Chen, and David Basin. PVLDB, 17(12): 4325 - 4328, 2024. [[paper](https://www.vldb.org/pvldb/vol17/p4325-liu.pdf)]

## 6. Database Diagnosis

### System and Kernel Causes

**Detecting Metadata-Related Logic Bugs in Database Systems via Raw Database Construction**

Jiansen Song, Wensheng Dou, Yu Gao, Ziyu Cui, Yingying Zheng, Dong Wang, Wei Wang, Jun Wei, and Tao Huang. PVLDB, 17(8): 1884 - 1897, 2024. [[paper](https://dl.acm.org/doi/10.14778/3659437.3659445)]

**When Amnesia Strikes: Understanding and Reproducing Data Loss Bugs with Fault Injection**

Maria Ramos, João Azevedo, Kyle Kingsbury, José Pereira, Tânia Esteves, Ricardo Macedo, and João Paulo. PVLDB, 17(11): 3017 - 3030, 2024. [[paper](https://www.vldb.org/pvldb/vol17/p3017-ramos.pdf)]

**Keep It Simple: Testing Databases via Differential Query Plans**

Jinsheng Ba and Manuel Rigger. SIGMOD 2024. [[paper](https://dl.acm.org/doi/10.1145/3654991)]

### Bottleneck Queries

## 7. General Techniques

### Feature Engineering for DB

**QCFE: An Efficient Feature Engineering for Query Cost Estimation**

Yu Yan, Hongzhi Wang, Junfang Huang, Dake Zhong, Tao Yu, Kaixin Zhang, Man Yang, Tianqing Wang. ICDE 2024. [[paper](https://ieeexplore.ieee.org/document/10597901)]

### Feature Engineering for Al



### Model Transfer

### Query And Data Generation

#### Query Generation

**Mirage: Generating Enormous Databases for Complex Workloads**

Qingshuai Wang, Hao Li, Zirui Hu, Rong Zhang, Chengcheng Yang, Peng Cai, Xuan Zhou, Aoying Zhou. ICDE 2024. [[paper](https://ieeexplore.ieee.org/document/10597682)]

---

#### Data Generation

**Differentially Private Data Generation with Missing Data**

Shubhankar Mohapatra, Jianqiao Zong, Florian Kerschbaum, and Xi He. PVLDB, 17(8): 2022 - 2035, 2024. [[paper](https://www.vldb.org/pvldb/vol17/p2022-mohapatra.pdf)]

**DB-MAGS: Multi-Anomaly Data Generation System for Transactional Databases**

Yiqi Shen, Sijia Li, Miaodong Shen, Peng Cai, Weiyuan Xu, Kai Li, and Jinlong Cai. PVLDB, 17(12): 4497 - 4500, 2024. [[paper](https://www.vldb.org/pvldb/vol17/p4497-shen.pdf)]

**SiloFuse: Cross-silo Synthetic Data Generation with Latent Tabular Diffusion Models**

A. Shankar, H. Brouwer, R. Hai and L. Chen. ICDE 2024. [[paper](https://ieeexplore.ieee.org/document/10597707)]



### Model Selection

**Database Native Model Selection: Harnessing Deep Neural Networks in Database Systems**

Naili Xing, Shaofeng Cai, Gang Chen, Zhaojing Luo, Beng Chin Ooi, Jian Pei. PVLDB, 17(5): 1020 - 1033, 2024. [[paper](https://dl.acm.org/doi/10.14778/3641204.3641212)]

## 8. Database Frameworks

**nsDB: Architecting the Next Generation Database by Integrating Neural and Symbolic Systems**

Ye Yuan, Bo Tang, Tianfei Zhou, Zhiwei Zhang, and Jianbin Qin. PVLDB, 17(11): 3283 - 3289, 2024. [[paper](https://www.vldb.org/pvldb/vol17/p3283-tang.pdf)]

**NeurDB: On the Design and Implementation of an AI-powered Autonomous Database**

Zhao, Z., Cai, S., Gao, H., Pan, H., Xiang, S., Xing, N., Chen, G., Ooi, B., Shen, Y., Wu, Y., & Zhang, M. (2024). ArXiv, abs/2408.03013. [[paper](https://arxiv.org/pdf/2408.03013)]

## 9. Demonstrations

**Demonstration of the VeriEQL Equivalence Checker for Complex SQL Queries**

Pinhan Zhao, Yang He, Xinyu Wang, and Yuepeng Wang. PVLDB, 17(12): 4437 - 4440, 2024. [[paper](https://www.vldb.org/pvldb/vol17/p4437-zhao.pdf)]
