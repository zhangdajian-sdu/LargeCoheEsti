# LargeCoheEsti

Supporting Code for "Scalable protocol for coherence estimation from scarce data: Theory and experiment"

## Introduction

This repository contains supporting code for the published paper:

> Qi-Ming Ding, Ting Zhang, Hui Li, and Da-Jian Zhang, **Scalable protocol for coherence estimation from scarce data: Theory and experiment**, *Physical Review A* **113**, 032444 (2026).

[Published article](https://doi.org/10.1103/g8sh-hts2) | [arXiv:2510.21138](https://arxiv.org/abs/2510.21138)

This repository is a fork of [geeeekDing/LargeCoheEsti](https://github.com/geeeekDing/LargeCoheEsti), the upstream repository.

It includes all the necessary code to reproduce the figures, generate the experimental data, and validate the algorithms presented in the paper.

## Code Structure

This repository is organized into two main parts: MATLAB and Python code. These are located in separate directories and are used to support the various experiments and analyses in our work.

## Requirements

Please ensure that your environment has the following prerequisites installed.

### MATLAB
To successfully run the MATLAB scripts, you will need the following toolboxes:

QETLAB：https://qetlab.com/

state_tomography：https://research.physics.illinois.edu/QI/Photonics/tomography/

CVX: https://cvxr.com/cvx/ A modeling system for constructing and solving disciplined convex programs.

CVXQUAD: https://github.com/hfawzi/cvxquad An extension for CVX that adds support for functions involving the matrix logarithm, exponential, and entropy.

Solver: We recommend using MOSEK as the solver for CVX to achieve the best performance and stability. However, other CVX-compatible solvers (e.g., SDPT3, SeDuMi) are also supported.

### Python
The Python environment requires the following standard scientific computing libraries: pandas numpy matplotlib torch scipy

You can quickly install these dependencies using pip:

pip install pandas numpy matplotlib torch scipy

## Usage
Data Generation & Algorithm Validation: These tasks are primarily handled by the MATLAB scripts. Please refer to the comments within the respective files for instructions on how to run them.

Figure Plotting: The figures are generated using Python scripts. These scripts read the data files (in .mat or .csv format) produced by MATLAB and create the plots shown in the paper.

## Citation

If you use this code or our methods in your research, please cite our paper:

```bibtex
@article{Ding2026CoherenceEstimation,
  author = {Ding, Qi-Ming and Zhang, Ting and Li, Hui and Zhang, Da-Jian},
  title = {Scalable protocol for coherence estimation from scarce data: Theory and experiment},
  journal = {Physical Review A},
  volume = {113},
  number = {3},
  pages = {032444},
  year = {2026},
  doi = {10.1103/g8sh-hts2},
  url = {https://doi.org/10.1103/g8sh-hts2},
  eprint = {2510.21138},
  archivePrefix = {arXiv},
  primaryClass = {quant-ph}
}
```

The repository's [CITATION.cff](CITATION.cff) also identifies this paper as the preferred citation.
