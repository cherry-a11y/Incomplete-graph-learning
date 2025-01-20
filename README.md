# Incomplete-graph-learning
This repository contains a curated list of papers focused on Incomplete Graph Learning . The papers are categorized based on their methodological contributions across Data-Level methods (Data Interpolation, Adversarial Generation, Pseudo-Labeling) and Algorithm-Level methods (Model and Training Refinement, Loss Function Engineering, Post-hoc Adjustments). Many papers contribute to multiple aspects, as indicated in their listings.
We aim to keep this list up to date. If you come across any errors or papers that should be included, please feel free to open an issue or submit a pull request.

# Outline

The outline corresponds to the taxonomy of Problems in our [survey paper](https://arxiv.org/abs/2308.13821).

- [1. Class Imbalance](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#1-class-imbalance)
  - [1.1 Node-Level Class Imbalance](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#11-node-level-class-imbalance)
    - [1.1.1 Imbalanced Node CLassification](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#111-imbalanced-node-classification)
    - [1.1.2 Node-Level Anomaly Detection](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#112-node-level-anomaly-detection)
    - [1.1.3 Few-Shot Node Classification](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#113-few-shot-node-classification)
    - [1.1.4 Zero-Shot Node Classification](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#114-zero-shot-node-classification)
  - [1.2 Edge-Level Class Imbalance](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#12-edge-level-class-imbalance)
    - [1.2.1 Few-Shot Link Prediction](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#121-few-shot-link-prediction)
    - [1.2.2 Edge-Level Anomaly Detection](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#122-edge-level-anomaly-detection)
    - [1.2.3 Imbalanced Link Classification](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#123-imbalanced-link-classification)
  - [1.3 Graph-Level Class Imbalance](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#13-graph-level-class-imbalance)
    - [1.3.1 Imbalanced Graph Classification](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#131-imbalanced-graph-classification)
    - [1.3.2 Graph-Level Anomaly Detection](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#132-graph-level-anomaly-detection)
    - [1.3.3 Few-Shot Graph Classification](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#133-few-shot-graph-classification)
- [2. Structure Imbalance](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#2-structure-imbalance)
  - [2.1 Node-Level Structure Imbalance](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#21-node-level-structure-imbalance)
    - [2.1.1 Imbalanced Node Degrees](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#211-imbalanced-node-degrees)
    - [2.1.2 Node Topology Imbalance](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#212-node-topology-imbalance)
    - [2.1.3 Long-Tail Entity Embedding on KGs](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#213-long-tail-entity-embedding-on-kgs)
  - [2.2 Edge-Level Structure Imbalance](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#22-edge-level-structure-imbalance)
    - [2.2.1 Few-Shot Relation Classification](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#221-few-shot-relation-classification)
    - [2.2.2 Zero-Shot Relation Classification](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#222-zero-shot-relation-classification)
    - [2.2.3 Few-Shot Reasoning on KGs](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#223-few-shot-reasoning-on-kgs)
  - [2.3 Graph-Level Structure Imbalance](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#23-graph-level-structure-imbalance)
    - [2.3.1 Imbalanced Graph Sizes](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#231-imbalanced-graph-sizes)
    - [2.3.2 Imbalanced Topology Groups](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#232-imbalanced-topology-groups)
- [3. Other Related Literature](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#3-other-related-literature)
  - [3.1 Fairness Learning on Graphs](https://github.com/Xtra-Computing/Awesome-Literature-ILoGs#31-fairness-learning-on-graphs)

# Introduction
# Preliminaries
## Taxonomy of graphs
### Taxonomy of the fundamental graphs
### Taxonomy of the incomplete graphs
## Relevant learning techniques
### Data imputation learning
### Label predication learning
### Graph representation learning
