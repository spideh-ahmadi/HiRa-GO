# HiRa-GO: Hierarchical Rainbow Community Detection in Gene Ontology Networks

This repository contains the official implementation of the HiRa-GO algorithm proposed in the paper:

**HiRa-GO: A Hierarchical Rainbow Community Detection Algorithm for Gene Ontology Networks**  


## Description

HiRa-GO is a DFS-based algorithm designed to detect hierarchical communities in directed ontology networks. It assigns colors to nodes by traversing the graph in post-order and propagating color labels based on leaf and internal node structure.

The method is especially suitable for biological networks such as the Gene Ontology and achieves better interpretability and lower structural entropy than modularity-based algorithms like Louvain.

## Contributors

This project was developed as a collaboration between:

- Sepideh Ahmadi — Idea, algorithm design, manuscript preparation  
- Dr. Javad Mohammadzadeh — Research supervision, co-author of the manuscript  
- Mr. Baghkhani — Code implementation and testing

## How to Run

1. Install required packages.

2. use the Jupyter Notebook:

jupyter notebook HiRa-GO.ipynb


## Evaluation

HiRa-GO was evaluated on the Gene Ontology dataset and compared with the Louvain algorithm. The proposed method showed significant improvements in structural entropy:

| Method   | Structural Entropy |
|----------|--------------------|
| Louvain  | 6.71               |
| HiRa-GO  | 3.23               |

## Dataset

The Gene Ontology dataset used in this study is in `go-basic.json` format and is available from the official GO website.

