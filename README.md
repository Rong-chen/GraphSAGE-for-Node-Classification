# GraphSAGE-for-Node-Classification
所有代码可直接在Colab运行
## 一、数据集
三类数据集：Cora, Citeseer, Pubmed
|Items|	Cora	|Citeseer|	Pubmed|
|  ----  | ----  |----|----|
|#Nodes|	2708|	3327|	19717|
|#Edges	|5429|	4732|44338|
|#Features|	1433|	3703|	500|
|#Classes|	7	|6	|3|
### 1.1 Cora数据集
2708个节点，5429条边。标签共7个类别。数据集的特征维度是1433维。

Cora数据集的节点是机器学习论文，论文主题（标签）分为以下七类之一：

Case_Based基于案例

Genetic_Algorithms遗传算法

Neural_Networks神经网络

Probabilistic_Methods概率方法

Reinforcement_Learning强化学习

Rule_Learning规则学习

Theory理论

论文的选择方式是，在最终语料库中，每篇论文引用或被至少一篇其他论文引用（即没有孤立点存在）。

### 1.2 CiteSeer数据集
CiteSeer数据集(引文网络)中，论文分为六类：

Agents

AI（人工智能）

DB（数据库）

IR（信息检索）

ML（机器语言）

HCI

共包含3312篇论文，记录了论文之间引用或被引用信息。去除停用词和在文档中出现频率小于10次的词，整理得到3703个唯一词。

### 1.3 Pubmed数据集
Pubmed数据集(引文网络)包括来自Pubmed数据库的19717篇关于糖尿病的科学出版物，分为三类：

Diabetes Mellitus, Experimental

Diabetes Mellitus Type 1

Diabetes Mellitus Type 2

引文网络由44338个链接组成。数据集中的每个出版物都由一个由500个唯一单词组成的字典中的TF/IDF加权词向量来描述。

## 二、实现方法

GraphSAGE

## 三、结果

|Dataset|	Cora	|Citeseer|	Pubmed|
|  ----  | ----  |----|----|
|Accuracy|	0.7790|	0.5660|	0.7510|
|F1_score	|0.7790|	0.5456|0.7519|
|AUC|	0.96|	0.85|	0.89|
