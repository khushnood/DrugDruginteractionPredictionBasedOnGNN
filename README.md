# GNN-based DDI Prediction

This repository contains code for the paper **Graph Neural Network-Based Drug-Drug Interaction Prediction**, which explores the use of Graph Neural Networks (GNNs) for predicting drug-drug interactions (DDIs) across various datasets.

---
extract the GnnbasedDrugDrugInteractionPrediction-github.zip file
## Environment Setup

To ensure reproducibility, all dependencies are listed in the `environment.yml` file. You can create the conda environment using:

```bash
conda env create -f environment.yml
conda activate gnn-ddi  # replace with the name defined in your .yml file

python src/main.py --model "gcn_skipconnection" --dataset "biosnapddi"

model choices: ["gcn_ngnn_graphconv", "sage_ngnn", "sage_skipconnection", "gcn", "sage", "gat_mlp", "gcn_skipconnection", "sage_nodefeature_mlp", "sage_mlp_virtual_node","magcn"]
data choices: ["ogbl-ddi", "drugbankddi","biosnapddi"]
For more information see the args help.
