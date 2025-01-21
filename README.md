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
* **Speedup robust graph structure learning with low-rank information** (*CIKM'21*) [[paper]](http://xiangliyao.cn/papers/cikm21-hui.pdf) [[code]](https://github.com/xh3204/LRGNN)
* **A survey on graph structure learning: Progress and opportunities** (*IJCAI22*) [[paper]](https://arxiv.org/pdf/2103.03036)
* **Matrix completion with cross-concentrated sampling: Bridging uniform sampling and CUR sampling.** (*IEEE Transactions on Pattern Analysis and Machine Intelligence*) [[paper]](https://arxiv.org/pdf/2208.09723) [[code]](https://github.com/huangl3/CCS-ICURC)
* **Onine learning for data streams with incomplete features and labels** (* IEEE Transactions on Knowledge and Data Engineering*) [[paper]](https://pdf.sciencedirectassets.com/271625/1-s2.0-S0020025524X00274/1-s2.0-S0020025524013252/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjELv%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLWVhc3QtMSJHMEUCIAZYcvULgGwiMFB6J7gjDtUGHXaNV92SrnyZDXPI%2FP%2FgAiEAuDia%2FqRc%2BAT28ScU4pgX5X%2FC8GuXp%2BaQn2nrSVX2b5IqugUItP%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FARAFGgwwNTkwMDM1NDY4NjUiDKGb9t%2BONxR5USjlACqOBWAkNyU32J2RQJa8dqqN7PQ3MtkbROvVEOUymqfTDmnYGZtZgArcSHaY2q%2FjpJC05C9euDIfJuEx1am1XzGNO9kGtUn0%2FeviyInQwvuWPiMdGdepeThI6jw%2BVxAUM%2FIZEt%2FPex%2FVS3eiFgwQnLIq8jWvRcrvRsVmBkyoPnG%2FyIrzpBO4b6pni11D820CuVkEHetRVH%2B5KpnfCHx5Nfdm14uKPBThLslWXlYKUayoRO%2FPB%2BcW9acbZhRQTv1dOcZVHBLDK0qF7kVS355gxkcCCih01n%2FBWMgrHMztUj4NpPeZriCAQokupgUQ7rt3c%2FtbbaZt1smi2DSpHwjc1lh5K%2BXrur9zvtGWXptEXFd6bQri0T9ndt%2B6cxdlWA5uYuyeNaYxx2upel63TPdh9UiiGIXfR4m7A3lBLpEk0o1WTaZu%2FuhUQbLr2W%2BUUpVsc54FDL5%2B6ZKhEFoNNQfweBmEwMAOUkrjpJ3Z6QmL6ucgVgim8p%2FoSFWHzh36rrGgA%2FKfW1MsDmMxF6PG3ehqRNG4H9i%2FfMhrmBNmU%2FRs77FXLs5jiMz%2Fk8q90G56xni55yeTkL28VEr8KRWSnX2Ot0hcAJ6ElnYitOLvFFvt7g3VUBUZfFVsb%2BYFbspwYm%2Fdbga2Dwp%2BG6D7LMIN3hQmh%2FMwtl1QVt%2Bvg6h35E3t9NrZ%2FwLDdAO51csLELPAb0wao9jN3vkqmmlXlNSqG%2BV4aJXHd6ayX1P4pl2GrNTt3qoDEBG8qiTfFAHb102orGCpC6%2F2w8EOGiRERfOvCwqvAa7qUZDN5%2BW5jtOLKVXovOwpwkGivRH%2BxPt3hPSbNF4Cb7lFoBwOsEfHi%2FzyjQLq9cAhKK5hjczZ4ikyhZqBw%2BUf7DDbkLy8BjqxAQmyZ7ZiHkddLhYcC%2FRAZRcVEOI0gsFb7nlJT2LcIn26Z%2BMQBH12ylmpl4w956Jek4Do118s5ovAMAHQ%2FOjFgUXUMYoGlO8VMDyzupgdkDKdMAQMxkdNq%2FouGIROQJJ4PC1jKIVCnlv2pxBJQakn1fphyqMWUReSW5hlSYvC1Dhan914VsYRIRJTTw6UwmflwcXl4dSbXCK4uuDqnEwAKQYkffY9nAehDzmET8PfcaFHQA%3D%3D&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20250121T033925Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTYZJA52AKL%2F20250121%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=435f8090f363b16f44038f9268ba0525be894be704f4866acbca51d4a8b1f9c1&hash=8354c811cb4ca08c5c99eec036a45e68b93edb22d6f9ad1f07c2bc3034cba389&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0020025524013252&tid=spdf-0e00855a-763f-4160-b5cb-9e9f3b0fa21d&sid=b2e916324c50074f488b0ff64cd23ad0cf5fgxrqa&type=client&tsoh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&ua=10165f5257545050030758&rr=905446ea9ad7d4b2&cc=jp) [[code]](https://github.com/youdianlong/OLIDSPLM)
*  **Robust rank-one matrix completion with rank estimation** (*Pattern Recognition*) [[paper]](https://pdf.sciencedirectassets.com/272206/1-s2.0-S0031320323X00065/1-s2.0-S0031320323003382/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjELv%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLWVhc3QtMSJHMEUCIAZYcvULgGwiMFB6J7gjDtUGHXaNV92SrnyZDXPI%2FP%2FgAiEAuDia%2FqRc%2BAT28ScU4pgX5X%2FC8GuXp%2BaQn2nrSVX2b5IqugUItP%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FARAFGgwwNTkwMDM1NDY4NjUiDKGb9t%2BONxR5USjlACqOBWAkNyU32J2RQJa8dqqN7PQ3MtkbROvVEOUymqfTDmnYGZtZgArcSHaY2q%2FjpJC05C9euDIfJuEx1am1XzGNO9kGtUn0%2FeviyInQwvuWPiMdGdepeThI6jw%2BVxAUM%2FIZEt%2FPex%2FVS3eiFgwQnLIq8jWvRcrvRsVmBkyoPnG%2FyIrzpBO4b6pni11D820CuVkEHetRVH%2B5KpnfCHx5Nfdm14uKPBThLslWXlYKUayoRO%2FPB%2BcW9acbZhRQTv1dOcZVHBLDK0qF7kVS355gxkcCCih01n%2FBWMgrHMztUj4NpPeZriCAQokupgUQ7rt3c%2FtbbaZt1smi2DSpHwjc1lh5K%2BXrur9zvtGWXptEXFd6bQri0T9ndt%2B6cxdlWA5uYuyeNaYxx2upel63TPdh9UiiGIXfR4m7A3lBLpEk0o1WTaZu%2FuhUQbLr2W%2BUUpVsc54FDL5%2B6ZKhEFoNNQfweBmEwMAOUkrjpJ3Z6QmL6ucgVgim8p%2FoSFWHzh36rrGgA%2FKfW1MsDmMxF6PG3ehqRNG4H9i%2FfMhrmBNmU%2FRs77FXLs5jiMz%2Fk8q90G56xni55yeTkL28VEr8KRWSnX2Ot0hcAJ6ElnYitOLvFFvt7g3VUBUZfFVsb%2BYFbspwYm%2Fdbga2Dwp%2BG6D7LMIN3hQmh%2FMwtl1QVt%2Bvg6h35E3t9NrZ%2FwLDdAO51csLELPAb0wao9jN3vkqmmlXlNSqG%2BV4aJXHd6ayX1P4pl2GrNTt3qoDEBG8qiTfFAHb102orGCpC6%2F2w8EOGiRERfOvCwqvAa7qUZDN5%2BW5jtOLKVXovOwpwkGivRH%2BxPt3hPSbNF4Cb7lFoBwOsEfHi%2FzyjQLq9cAhKK5hjczZ4ikyhZqBw%2BUf7DDbkLy8BjqxAQmyZ7ZiHkddLhYcC%2FRAZRcVEOI0gsFb7nlJT2LcIn26Z%2BMQBH12ylmpl4w956Jek4Do118s5ovAMAHQ%2FOjFgUXUMYoGlO8VMDyzupgdkDKdMAQMxkdNq%2FouGIROQJJ4PC1jKIVCnlv2pxBJQakn1fphyqMWUReSW5hlSYvC1Dhan914VsYRIRJTTw6UwmflwcXl4dSbXCK4uuDqnEwAKQYkffY9nAehDzmET8PfcaFHQA%3D%3D&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20250121T034607Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTYZJA52AKL%2F20250121%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=d26d8336aecef28d053b0a4115c56cf6c5c9cf08a3aae99c73f41a377dcbd488&hash=c70a732d6af3c8a7d48bc47dea0bfe45ccc1928af0cd338be13abc273abccb5a&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0031320323003382&tid=spdf-e65432f6-9b7e-4534-8d4f-5e0b8dff138b&sid=b2e916324c50074f488b0ff64cd23ad0cf5fgxrqa&type=client&tsoh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&ua=10165f5257545156045e05&rr=905450b8d85cd561&cc=jp) 





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

