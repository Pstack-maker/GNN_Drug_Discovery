# GNN Drug Discovery Pipeline

Overview:

This is my project exploring the use of Graph Neural Networks (GNNs) for predicting key drug discovery properties like **lipophilicity**, **solubility**, and **blood-brain barrier permeability**.  
I ran into a lot of issues getting RDKit to work locally (NumPy and version conflicts), so I used Claude to help generate the molecular graph representations. 
Designed to run in **Google Colab**.

Approach:

Instead of building separate models for each property, this project uses multi-task learning where one model learns shared chemical knowledge that helps with all predictions. The architecture includes:

-Graph Attention Networks (GAT) for molecular understanding
-Shared representation learning across tasks
-Task-specific prediction heads for each property
-Real pharmaceutical datasets from DeepChem and ChEMBL

- `notebooks/` — Colab notebook with full pipeline
- `data/` — input data (add your own)
- `results/` — output plots and metrics
- `models/` — saved models

Requirements:

**Python 3.9**

Install dependencies with:

  ```bash
  pip install -r requirements.txt

Clone this repo:

```bash
git clone https://github.com/<your-username>/GNN-Drug-Discovery.git