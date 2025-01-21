# Incomplete-graph-learning
This repository contains a curated list of papers focused on Incomplete Graph Learning . The papers are categorized based on their methodological contributions across Data-Level methods (Data Interpolation, Adversarial Generation, Pseudo-Labeling) and Algorithm-Level methods (Model and Training Refinement, Loss Function Engineering, Post-hoc Adjustments). Many papers contribute to multiple aspects, as indicated in their listings.
We aim to keep this list up to date. If you come across any errors or papers that should be included, please feel free to open an issue or submit a pull request.

# Outline

The outline corresponds to the taxonomy of Problems in our [survey paper](https://arxiv.org/abs/2308.13821).

- [Introduction](https://github.com/cherry-a11y/Incomplete-graph-learning/blob/main/README.md#introduction)
- [Preliminaries](https://github.com/cherry-a11y/Incomplete-graph-learning/blob/main/README.md#preliminaries)
  - [Taxonomy of graphsl Structure Imbalance](https://github.com/cherry-a11y/Incomplete-graph-learning/blob/main/README.md#taxonomy-of-graphs)
    - [Taxonomy of the fundamental graphs](https://github.com/cherry-a11y/Incomplete-graph-learning/blob/main/README.md#taxonomy-of-the-fundamental-graphs)
    - [Taxonomy of the incomplete graphs](https://github.com/cherry-a11y/Incomplete-graph-learning/blob/main/README.md#taxonomy-of-the-incomplete-graphs)
  - [Relevant learning techniques](https://github.com/cherry-a11y/Incomplete-graph-learning/blob/main/README.md#relevant-learning-techniques)
    - [Data imputation learning](https://github.com/cherry-a11y/Incomplete-graph-learning/blob/main/README.md#data-imputation-learning)
    - [Label predication learning](https://github.com/cherry-a11y/Incomplete-graph-learning/blob/main/README.md#label-predication-learning)
    - [Graph representation learning](https://github.com/cherry-a11y/Incomplete-graph-learning/blob/main/README.md#graph-representation-learning)
  - [2.3 Graph-Level Structure Imbalance](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#23-graph-level-structure-imbalance)
    - [2.3.1 Imbalanced Graph Sizes](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#231-imbalanced-graph-sizes)
    - [2.3.2 Imbalanced Topology Groups](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#232-imbalanced-topology-groups)
- [3. Other Related Literature](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#3-other-related-literature)
  - [3.1 Fairness Learning on Graphs](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#31-fairness-learning-on-graphs)

# Introduction
* **Dual graph networks with synthetic oversampling for imbalanced rumor detection on social media** (*WWW'24*) [[paper]](https://doi.org/10.1145/3589335.3651494)
* **Learning to reconstruct missing data from spatiotemporal graphs with sparse observations** (*NeurIPS 2022*) [[paper]](https://arxiv.org/pdf/2205.13479) [[code]](https://github.com/Graph-Machine-Learning-Group/spin)
* **Handling missing data with graph representation learning** (*NeurIPS 2020*) [[paper]](https://arxiv.org/pdf/2010.16418) [[code]](https://github.com/maxiaoba/GRAPE)
* **Gapformer: Graph transformer with graph pooling for node classification** (*IJCAI-23*) [[paper]](https://www.ijcai.org/proceedings/2023/0244.pdf)
* **Time-aware gradient attack on dynamic network link prediction** (*IEEE TRANSACTIONS ON KNOWLEDGE AND DATA ENGINEERING*) [[paper]](https://zhichen98.github.io/data/TKDE2023-TGA.pdf)
* **Learning aligned vertex convolutional networks for graph classification** (*IEEE TNNLS*) [[paper]](https://arxiv.org/pdf/1902.09936) [[code]](https://github.com/maxiaoba/GRAPE)
* **Distributed large-scale natural graph factorization** (*WWW2013*) [[paper]](https://static.googleusercontent.com/media/research.google.com/en/us/pubs/archive/40839.pdf)
* **SCAN: a structural clustering algorithm for networks** (*KDD'07*) [[paper]](https://www1.se.cuhk.edu.hk/~hcheng/seg5010/slides/p824-xu.pdf) [[code]](https://github.com/rdmpage/scan-structural-clustering)
* **Do birds of a feather watch each other?: Homophily and social surveillance in location based social networks** (*CSCW'15*) [[paper]](https://dl.acm.org/doi/10.1145/2675133.2675179) 
* **A comprehensive survey on deep graph representation learning** (*Neural Networks*) [[paper]](https://arxiv.org/pdf/2304.05055)
* **Graph learning: A comprehensive survey and future directions** (*2022*) [[paper]](https://arxiv.org/pdf/2212.08966v1)
* **Learning on attribute-missing graphs** (*IEEE TRANSACTIONS ON PATTERN ANALYSIS AND MACHINE INTELLIGENCE*) [[paper]](https://arxiv.org/pdf/2011.01623) [[code]](https://github.com/xuChenSJTU/SAT-master-online)
* **Analyzing heterogeneous networks with missing attributes by unsupervised contrastive learning** (* IEEE Transactions on Neural Networks and Learning Systems*) [[paper]](https://ieeexplore.ieee.org/document/9724614) [[code]](https://github.com/liangchundong/HGCA)
* **Speedup robust graph structure learning with low-rank information.** (*CIKM'21*) [[paper]](http://xiangliyao.cn/papers/cikm21-hui.pdf) [[code]](https://github.com/xh3204/LRGNN)
* **A survey on graph structure learning: Progress and opportunities.** (*IJCAI22*) [[paper]](https://arxiv.org/pdf/2103.03036)
* 





# Preliminaries
## Taxonomy of graphs
### Taxonomy of the fundamental graphs
### Taxonomy of the incomplete graphs
## Relevant learning techniques
### Data imputation learning
### Label predication learning
### Graph representation learning
# Attribute-incomplete graph methods
## Data imputation methods
### Traditional matrix completion methods
### Graph learning methods
## Label predication methods
# Attribute-missing graph learning methods
## Data imputation methods
### Data imputation methods on homogeneous graphs
### Data imputation methods on heterogeneous graphs
## Label predication methods
# Hybrid-absent graph learning methods
# Incomplete graph learning in practice
## Datasets
### Non-graph structured datasets
### Graph structured datasets
## Incomplete processing mode
## Evaluation index
### Node classification
### Node clustering
### Link prediction
### Feature estimation
## Applications
### Knowledge graphs
### Transportation systems
### Recommendation systems
### Summary and discussion
# Discussion and conclusion
## Discussion
### Interpretability and robustness
### Complex types of graphs
### Learning with multiple pretext tasks
### Broader scope applications
## Conclusion

