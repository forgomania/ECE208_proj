# Structural Protein Sequences Analysis
#### Yijing Li / Zhenghong Ma / Weixin Li / Weinan Li
## Purpose
Secrets about creatures including human beings is hidden in the protein sequences. Our team decided to explore the hidden information inside the protein sequences by analyzing more than 400,000 protein structure sequences and give insights to protein classification. We focus on one-dimensional structure of protein. Based on that we classify proteins by basic physical and chemical characteristics, hydrophobicity and transmembrane domain structures of proteins.
## Dataset
We are going to use a protein data set retrieved from Research Collaboratory for Structural Bioinformatics (RCSB) Protein Data Bank (PDB). It contains protein metadata which includes details on protein classification, extraction methods, experimental technique, etc. There are two data files which are both arranged by structureId. In order to analyze problems more specifically, we plan to do data cleaning first. For example, we need to exclude some small fragments of DNA in the dataset.
## Draft of Proposed Solution
### Neural Network
• Model: We consider using deep neural networks and LSTMs for the classification task.
• Training: Pass the input data through all layers in forward, then pass the error in backward pass.
• Error: Put the test set into a forward pass then we can get the prediction by the Neural Network.
### Hidden Markov Model
• Design the structure of HMMs from the training data, including insertion, deletion and match.
• Implement EM algorithm to tune the parameters and estimate the transition and emission matrices.
• Based on the Viterbi algorithm, forward and backward algorithm, get the probability of the test data.
### Support Vector Machine
• Soft margin (allow some deviation)
• Kernel (higher-dimension projection)
## Experimental Steps
1. Deal with the data:
For the processed dataset, use a split 80% train, 10% holdout and 10% test.
2. Build different classification models:
Adopt different machine learning methods mentioned above.
3. Comparison and summary:
Compare and evaluate in the aspect of algorithm accuracy and efficiency.
Analyze the comparison result and give a summary review as well as future suggestion.
