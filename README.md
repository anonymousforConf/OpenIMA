# OpenIMA
The PyTorch implementation of OpenIMA.

OpenIMA is proposed for open-world semi-supervised learning for node classification.

# Overview
Specifically, the repository is organized as follows:

* `losses/` contains the implementation of supervised contrastive loss, which can be used for implementing the proposed PLCL loss.

* `networks/` contains the implementation of a GAT backbone.

* `networks_large/` contains the implementation of a GAT backbone for large graph datasets.
 
* `util.py` is used for loading and pre-processing the dataset, and also includes the functions for computing metrics.

* `train_ours.py` is used for implementing the pipeline of OpenIMA.

* `train_ours_large.py` is used for implementing the pipeline of OpenIMA for large graph datasets.

# Running the code
To run OpenIMA on the example dataset Coauthor CS
```
$ cd run/
$ sh run_ours.sh
```

To run OpenIMA on the larger example dataset ogbn-arxiv
```
$ cd run/
$ sh run_ours_large.sh
```
All the experiments are repeated ten times under ten different data splits, and the reported accuracy is averaged over the ten runs.
