# Single-Cell-Perturbations
Predict gene expressions in different cell types after small molecule perturbations

## Model Design

Heterogeneous graph is created with two types of nodes - **Cell type nodes** and **Small molecule nodes**. Each pair of (cell type, small molecule) nodes have an undirected edge.

![image](https://github.com/user-attachments/assets/072fe41f-51ad-4143-9f67-628edd3ec2c7)

## Node Embedding

![image](https://github.com/user-attachments/assets/b1c51c47-4ba6-417a-8654-9b1c7451713f)

## Prediction

For each pair of (cell type, small molecule) nodes, the perturbation prediction is made by concatenating their respective node embeddings and passing through one to several linear layers.

![image](https://github.com/user-attachments/assets/cb6bd62d-0edc-42b9-8011-4167887869f7)

## Leverage Multiome Gene Expression Data
![image](https://github.com/user-attachments/assets/27747a88-6fcb-4745-ad98-0c8d9c7244c7)
