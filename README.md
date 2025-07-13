# (2,2)_GB-Codes_Classification
This repository provides a comprehensive classification of (2,2)-Generalized Bicycle (GB) codes, of length less than 200. This work rigorously identifies these codes up to an equivalence relation compatible with their CSS code structures and Cayley graph properties.


## Table of Contents
- [About GB Codes](#about-gb-codes)
- [Classification Methodology](#classification-methodology)
- [Repository Structure](#repository-structure)
- [How to Use/Reproduce](#how-to-usereproduce)
- [Results](#results)
- [Citation](#citation)


## About Generalized Bicycle (GB) Codes
(2,2)-Generalized Bicycle codes are a specialized type of CSS codes derived from from pairs of binary circulant matrices with two non-zero elements per row, intrinsically linked to Cayley graphs. 
They are known for their efficient encoding and decoding properties, making them promising candidates for practical quantum error correction. 


## Classification Methodology
The equivalence relation used in this classification corresponds to 2-isomorphisms between the underlying Cayley graphs.
Our classification focused exclusively on elementary GB codes of the form $GB(1 + X^a, 1 + X^b, n)$ with $gcd(a, b, n) = 1$, as these serve as the fundamental building blocks for all (2,2)-GB codes. The computational aspects were performed using **SageMath** and **Magma**. SageMath was utilized for determining equivalence classes of isomorphic graphs and evaluating their k-connectivity. Magma was employed for computing the minimum distance of the quantum codes. For codes with identical parameters, manual verification for non-2-isomorphism was conducted by checking 3-connectivity of underlying graphs (where applicable, per Whitney's Theorem on 3-connected graphs) or by verifying non-permutation equivalence of row spaces of incidence matrices.


## Repository Structure
This repository is organized as follows:
- `scripts/`: Contains SageMath and Magma scripts used for graph isomorphism checking, k-connectivity analysis and minimum distance computation of quantum codes.
- `results_data/`: Processed lists of classified codes.
- `README.md`: This file.
  

## How to Use/Reproduce
To reproduce the results or utilize the scripts in this repository, you will need:
-   **SageMath:** accessible via JupyterNotebook
-   **Magma:** https://magma.maths.usyd.edu.au/magma/
  

## Results
The main outcomes of this classification are detailed in the `results_data/` file. This includes a comprehensive list of distinct (2,2)-GB codes, presented for each set of parameters [[2n, 2, d]] with n ranging from 1 to 100. For any given parameter set, we provide all non-equivalent GB codes corresponding to it.


## Citation 
If you use the data or code from this repository in your research, please cite the associated paper. The full citation will be provided here once the paper is published.

```latex
@article{ArnaultGaboritSaussay:GBcodes_in_prep,
  title={{(2,2)-GB Codes: Classification and Comparison with weight-4 Surface Codes}},
  author={Arnault, François and Gaborit, Philippe and Saussay, Nicolas},
  note={Manuscript in preparation},
  year={2025}
}
