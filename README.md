# PyTorch implementation of GCN and GAT on Cora

The notebook is organised as follows:
1. The [Cora](https://arxiv.org/abs/1603.08861) dataset
2. [GCN](https://arxiv.org/abs/1609.02907): we build our own `pytorch_geometric.nn.GCNConv` layer.
2. [GAT](https://arxiv.org/abs/1710.10903): we build our own `pytorch_geometric.nn.GATConv` layer.

The main idea of this project is to learn how the GCN and GAT layers could be implemented in practice. Thus, the presented implementations are not too naive, but also not extremely optimized. If you don't have time to disect the [PyG documentation](https://pytorch-geometric.readthedocs.io/en/latest/index.html) and still want an useful GCN or GAT code, then you might want to check the notebook.

## Setup

1. Clone this repository
```
git clone https://github.com/arturtoshev/from_gcn_to_gat.git 
cd from_gcn_to_gat
```
2. Create a virtual environment using `virtualenv` or 
```
python3 -m venv ./venv
source venv/bin/activate
```
3. You can work on the code with or without CUDA. 
    - If you want to work with CUDA, you need the torch version corresponding to your cuda installation, see [here](https://pytorch.org/get-started/locally/). For CUDA 11.1 and torch 1.9.1 you can run `pip install -r requirements_cu111.txt`
    - If you don't mind waiting a couple of extra second or don't have CUDA, then try `pip install -r requirements.txt`, which is based on torch 1.9.1. Caution: CPU installation NOT TESTED!


## Licence

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

