# Accurate Drug-Target Interaction Prediction using Deep Learning Architectures

## Project Overview

This project focuses on enhancing Drug-Target Interaction (DTI) prediction, a crucial step in drug repurposing and discovery. DTI prediction aims to identify potential therapeutic interactions between existing drugs and disease targets, offering a faster and more cost-effective alternative to traditional drug development. We explore the application of advanced deep learning models to overcome the limitations of time-consuming and resource-intensive experimental methods.

## The Problem

Traditional methods for identifying Drug-Target Interactions are heavily reliant on biological experiments and heuristic algorithms. These approaches are often costly, time-consuming, and resource-intensive, significantly slowing down the drug discovery process. There is a pressing need for efficient, accurate, and scalable computational methods to predict DTI.

## Solution Finding

Our approach investigates two distinct deep learning architectures for DTI prediction:

1.  **Multi-Layer Graph Attention Networks (MLGANNs)**: This method models drugs and targets as nodes in a graph, with their interactions or similarities forming the edges. MLGANNs leverage attention mechanisms to prioritize important interactions within this graph, effectively capturing complex relationships.
2.  **BERT-based Models**: Building on transformer architectures, these models are adept at recognizing intricate patterns within sequential data. They process drug sequences (SMILES strings) and protein sequences (amino acid sequences) to generate meaningful representations, enabling precise DTI outcome predictions.

## Key Improvements and Contributions

Our research involved developing and fine-tuning these models, leading to several notable improvements:

* **Enhanced MLGANN with Heterogeneous Graph Fusion**: We designed an MLGANN DTI layer as a heterogeneous graph, integrating multiple biological data sources such as chemical structure, side-effect relationships, disease associations, and protein interactions. This fusion enhances prediction accuracy by capturing relationships both within and across different data types, and a dual attention mechanism dynamically prioritizes clinically relevant layers.
* **BERT Model with Subsequence Embedding**: We preprocess drug and protein sequences by encoding them into informative embeddings using techniques like the Frequent Consecutive Subsequence (FCS) algorithm for drugs. These embeddings are then fed into a pre-trained BERT model, which learns contextual relationships through its transformer encoder layers.
* **Enhanced BERT Model using Association Rule Mining (ARM)**: To further boost the BERT model's performance, we incorporated Association Rule Mining as a preprocessing step. ARM helps identify critical patterns in subsequence interactions that are indicative of successful drug-target bindings, guiding the BERT model's attention mechanism and refining prediction probabilities.
* **Demonstrated Importance of Structural Information**: Across both MLGANN and BERT models, our experiments consistently showed that integrating structural and relational information (e.g., through adjacency matrices or association rules) significantly improves prediction performance.
* **Superior Performance of Domain-Specific Models**: Comparisons highlighted that domain-specific pretraining, such as using BioBERT over a general-purpose BERT model, leads to markedly better performance on DTI prediction tasks, showcasing the value of incorporating biomedical domain knowledge.

## Contributors

This project was a collaborative effort. The contributors include:
* Ishita Godani
* Neha Mutalik Desai 
* Arul Bhardwaj 
* Naman Bhatia
