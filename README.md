# Joint Network-and-Server Congestion in Multi-Source Traffic Allocation

This repository contains the Python implementation and reproducibility materials for:

**Joint Network-and-Server Congestion in Multi-Source Traffic Allocation: A Convex Formulation and Price-Based Decentralization**
Tamoghna Sarkar and Bhaskar Krishnamachari, WiOpt 2026.

* [IEEE publication](https://doi.org/10.23919/WiOpt71098.2026.11568243)
* [Initial arXiv version](https://arxiv.org/abs/2602.03246)

## Overview

The work studies traffic allocation from multiple sources to multiple service nodes when congestion arises jointly on the source-to-node access paths and at the service nodes themselves. It formulates flow-weighted end-to-end delay minimization as a convex optimization problem and derives a Wardrop-type characterization based on total marginal-cost equalization.

The repository implements:

* The centralized convex optimization benchmark.
* The synchronous price-based distributed routing algorithm.
* A common feasibility step that protects shared service-node capacities.
* KKT, Wardrop, conservation, capacity, price-consistency, and fixed-point checks.
* Convergence, utilization, routing, and per-source delay visualizations.
* A windowed stochastic count experiment for evaluating noisy load tracking and routing adaptation.

## Running the Notebook

The implementation is provided as a Jupyter notebook. The main dependencies are:

```bash
pip install numpy pandas scipy matplotlib seaborn jupyter
```

Launch Jupyter and run the notebook from top to bottom:

```bash
jupyter notebook WiOpt26JNSC.ipynb
```

The notebook generates the centralized and distributed solutions, numerical residual certificates, and the figures used in the extended manuscript.

## Citation

If you use this code or build on this work, please cite:

```bibtex
@INPROCEEDINGS{11568243,
  author={Sarkar, Tamoghna and Krishnamachari, Bhaskar},
  booktitle={2026 24th International Symposium on Modeling and Optimization in Mobile, Ad Hoc, and Wireless Networks (WiOpt)},
  title={Joint Network-and-Server Congestion in Multi-Source Traffic Allocation: A Convex Formulation and Price-Based Decentralization},
  year={2026},
  volume={},
  number={},
  pages={1-8},
  keywords={Delays;Pricing;Modeling;Costing;Costs;Algorithms;Equations;Loading;Stars;Optimization;rate allocation;traffic allocation;convex optimization;queueing delay;load balancing;marginal cost pricing;Wardrop condition;distributed algorithm},
  doi={10.23919/WiOpt71098.2026.11568243}
}
```
