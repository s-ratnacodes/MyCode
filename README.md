# MyCode

# TAGII

**TAGIIConv** is a Graph Neural Network (GNN) architecture designed for graph-based learning tasks. This repository contains the implementation of TAGII along with the required experimental files, datasets, and ablation study.

> **Note:** A detailed description of the architecture, mathematical formulation, and experimental results will be added soon.

---

## 📌 Overview

Graph Neural Networks (GNNs) have become an important class of models for learning representations from graph-structured data. **TAGII** is proposed as a GNN architecture with the goal of improving graph representation learning. The proposed TAGII is a simple yet a powerful extension of TAGCN that extends vanilla TAGCN effienciently by adding a teleport probability in the convolution formula. The teleport term has been borrowed from the Personalized PageRank scheme of APPNP. The same idea was later adopted as the initial residual in GCNII. It simply helps to reduces over-smoothing problem. The additional computational overhead is almost negligible. The rigrous experimentation conducted on standard node classification datasets and it clearly shows improved performance over the baseline TAGCN.

The repository provides:

* The implementation of **TAGII**
* Training and evaluation scripts
* Experimental configurations
* An ablation study
* Support for datasets available through **PyTorch Geometric (PyG)**

---


## 📂 Repository Structure

The repository is organized as follows:

```text
.
├── test.py
├── test2.py
├── test3.py
├── test4.py
├── test5.py
├── ab1.py
└── README.md
```



## 📊 Datasets

The datasets used in this repository are available through **PyTorch Geometric (PyG)**.

PyTorch Geometric provides a collection of commonly used graph datasets that can be directly loaded using its dataset classes.

Official documentation:

**PyTorch Geometric:**
https://pytorch-geometric.readthedocs.io/

### Dataset Installation

Install PyTorch Geometric and its dependencies according to the official installation instructions:

```bash
pip install torch-geometric
```

Then, the datasets can be loaded using the corresponding PyG dataset classes.

For example:

```python
from torch_geometric.datasets import <DatasetName>

dataset = <DatasetName>(root="./data")
```

Replace `<DatasetName>` with the dataset used in the paper.

---

## ⚙️ Installation

Clone the repository:

```bash
git clone <YOUR-GITHUB-REPOSITORY-URL>
cd <REPOSITORY-NAME>
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

If a `requirements.txt` file is not provided, install the main dependencies manually:

```bash
pip install torch torch-geometric
```

For the recommended PyTorch/PyG installation, please refer to the official PyTorch Geometric documentation.

---

## 🚀 Usage

### Training/Evaluatiom

To train/evaluate TAGII, run these .ipynb files in your colab/ jupyter notebook notebook.


## 🔬 Ablation Study

The repository also includes an **ablation study** to investigate the contribution of individual components of TAGII.

The ablation implementation is provided in: ab1.ipynb file


---


## 🧪 Reproducibility

To reproduce the experiments reported in the paper/repository:

1. Install the required dependencies.
2. Download/load the datasets through PyTorch Geometric.
3. Select the desired dataset and experimental configuration.
4. Run the corresponding training script.
5. Evaluate the trained model using the evaluation script.
6. Run `ablation.py` to reproduce the ablation experiments.


Note: use exactly same random seeds, hyperparameters, hardware configuration, and exact commands for same results.

---

### 🖥️ Hardware and Software Environment

All experiments were conducted on a **Linux-based machine** with the following configuration:

| Component        | Specification                  |
| ---------------- | ------------------------------ |
| Operating System | Linux                          |
| Kernel           | 6.8.0-136-generic              |
| Architecture     | x86_64                         |
| glibc            | 2.35                           |
| Python           | 3.12.7                         |
| PyTorch          | 2.5.1+cu121                    |
| CUDA             | 12.1                           |
| GPU              | NVIDIA RTX 2000 Ada Generation |
| GPU Count        | 1                              |

All models were trained on a **single NVIDIA RTX 2000 Ada Generation GPU** using CUDA 12.1.

---

## 📚 Citation

If you find **TAGII** useful in your research, please do not forget to cite us. Thanks!



> **S Ratna¹***, **Sukhdeep Singh²**, **Anuj Sharma¹**. TAGII: Topology Adaptive Graph Convolution Network using Teleport Probability. Manuscript under review.**

A formal citation will be provided once the paper is published.

## 👥 Authors

**S Ratna¹***, **Sukhdeep Singh²**, **Anuj Sharma¹**

¹ Department of Computer Science and Applications, Panjab University, Chandigarh, India


² Department of Computer Science, D.M. College, Moga (affiliated to Panjab University), Punjab, India

* Corresponding author

---







## 🤝 Acknowledgements


* The research work is conducted at DCSA, Panjab University, Chandigarh, India.
* PyTorch Geometric: https://pyg.org/
* PyTorch: https://pytorch.org/


---


