# 🧠 Hybrid GNN Architectures for Multi-Modal Protein–Ligand Interface Affinity Prediction

![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)
![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-red)
![PyTorch Geometric](https://img.shields.io/badge/PyTorch%20Geometric-GNN-orange)
![RDKit](https://img.shields.io/badge/RDKit-Chemoinformatics-green)
![Biopython](https://img.shields.io/badge/Biopython-Structural%20Biology-teal)
![License](https://img.shields.io/badge/License-MIT-lightgrey)
![Status](https://img.shields.io/badge/Status-Ongoing%20Research-yellow)

A **hybrid, multi-modal graph neural network framework** for predicting **protein–ligand interface binding affinity** by jointly modeling **structural, physicochemical, and sequence-derived features**.

---

## 🚀 Overview

This project explores **hybrid GNN architectures** that integrate **multiple biological modalities** to improve protein–ligand binding affinity prediction. Unlike single-representation models, this framework explicitly captures **interface-level interactions** by fusing:

- 3D structural graphs  
- Sequence-based embeddings  
- Physicochemical and geometric descriptors  

The model is designed to learn **complementary representations** across modalities and reason over their interactions using attention-based fusion mechanisms.

---

## ✨ Key Features

- 🧬 **Multi-modal representation learning**
  - 3D protein–ligand structural graphs  
  - Sequence-derived embeddings (protein & ligand)  
  - Physicochemical and geometric descriptors  

- 🔗 **Hybrid GNN architectures**
  - Graph convolution + graph attention layers  
  - Transformer-based cross-modal fusion  
  - Interface-aware message passing  

- 🧠 **Explicit interface modeling**
  - Residue–atom interaction graphs  
  - Distance- and contact-based edge construction  

- 🔍 **Interpretability**
  - Attention maps over residues and ligand atoms  
  - Modality contribution analysis  

- 📊 Trained on large-scale protein–ligand affinity datasets (e.g., PDBbind)

---

## 📁 Repository Structure

.
├── data/
│ ├── structures/ # PDB and MOL2 files
│ ├── sequences/ # Protein & ligand sequences
│ └── processed/ # Serialized graph objects
│
├── scripts/
│ ├── preprocess/ # Graph & feature generation
│ ├── train.py
│ └── evaluate.py
│
├── models/
│ ├── gnn_layers/
│ ├── fusion_modules/
│ └── hybrid_models.py
│
├── notebooks/
│ └── analysis.ipynb
│
├── results/
│ ├── metrics/
│ └── visualizations/
│
└── README.md


---

## ⚙️ Installation

### Requirements
- Python **3.8+**
- PyTorch
- PyTorch Geometric
- RDKit
- Biopython
- NetworkX
- NumPy / SciPy

### Install Dependencies

```bash
pip install torch torchvision torchaudio
pip install torch-geometric rdkit-pypi biopython networkx numpy scipy
```
### ▶️ Usage
Prepare data:
```
Protein structures (PDB)
Ligand structures (MOL2)
Protein sequences (FASTA)
```
Preprocess and generate graphs:
```
python scripts/preprocess/generate_graphs.py
```
Train hybrid GNN model:
```
python scripts/train.py
```
Evaluate and interpret:
```
python scripts/evaluate.py
```
## 📊 Dataset

Primary Dataset: PDBbind
Scale: ~9,000+ protein–ligand complexes
Labels: Experimental binding affinity values
Focus: Interface-level interactions

## 🧠 Research Contributions
Demonstrates the benefit of multi-modal fusion over single-graph models

Introduces interface-aware hybrid GNNs

Provides interpretable insights into residue–ligand interaction mechanisms

## 📬 Contact
For collaborations or questions:

Open a GitHub issue

Or email: sravyasri.mallampalli@gmail.com

## 📄 License
This project is licensed under the MIT License.

⭐ If you find this repository useful, please consider starring it!

## 🏗️ Architecture Overview

