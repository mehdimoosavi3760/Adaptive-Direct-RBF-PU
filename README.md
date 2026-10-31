# A Condition-Controlled Adaptive Direct RBF-PU Meshless Solver

**MATLAB Codes and Numerical Experiments**

## Overview

This repository contains MATLAB implementations and numerical experiments associated with the research paper:

**A Condition-Controlled Adaptive Direct RBF-PU Meshless Solver**

The study proposes a condition-controlled adaptive framework for the Direct Radial Basis Function Partition of Unity (D-RBF-PU) method for the efficient and stable numerical solution of elliptic partial differential equations (PDEs).

The proposed framework combines Adaptive Residual Subsampling (ARS) with a condition-triggered Hybrid Variably Scaled Kernel (HVSK) strategy.

The main objective is to improve numerical accuracy and stability while controlling the growth of local condition numbers during adaptive refinement.

Unlike the standard RBF-PU formulation, the Direct RBF-PU approach avoids the differentiation of partition of unity weight functions, resulting in a computationally efficient formulation.

## Main Contributions

The proposed framework incorporates the following features:

- **Direct RBF-PU formulation:** Avoids the costly differentiation of partition of unity weight functions.
- **Adaptive Residual Subsampling (ARS):** Refines the node distribution in regions requiring higher resolution.
- **Condition-controlled stabilization:** Monitors local collocation matrix condition numbers.
- **Hybrid Variably Scaled Kernels (HVSK):** Activates variable scale functions only in critically ill-conditioned patches while retaining standard kernels in well-conditioned regions.
- **Numerical stability:** Controls local ill-conditioning during adaptive refinement.
- **Computational efficiency:** Reduces the number of required nodes and computational time compared with non-adaptive D-RBF-PU and classical residual-driven adaptive approaches.

## Radial Basis Functions

The numerical implementations investigate three radial basis function families:

1. **Gaussian (GA)**
2. **Matérn**
3. **Thin Plate Spline (TPS)**

The adaptive and stabilization strategies are investigated using these kernels.

## Mathematical Problems

The numerical experiments focus on elliptic partial differential equations, particularly Poisson problems involving:

- Multi-peak solutions.
- Sharp-peak solutions.
- Oscillatory solutions.
- Problems with steep spatial gradients.

Both regular and irregular computational domains are considered in the numerical investigations.

## Repository Structure

```text
Adaptive-Direct-RBF-PU/
│
├── README.md
│
├── MATLAB_Codes.rar
│
├── Manuscript/
│
├── Figures/
│
└── Numerical_Results/
```

## Numerical Evaluation

The performance of the proposed method is evaluated using several numerical criteria:

- Root Mean Square Error (RMSE).
- Global condition number.
- Maximum local condition number.
- Number of computational nodes.
- Matrix sparsity.
- Matrix assembly time.
- Linear system solution time.
- Cumulative computational time.

Comparisons are performed between non-adaptive D-RBF-PU, classical residual-driven adaptive approaches, and the proposed condition-controlled adaptive framework.

## Theoretical Analysis

The theoretical contributions include:

- Optimal local approximation rates under the HVSK framework.
- A controlled bound for the global condition number in terms of local condition numbers.
- Quasi-linear computational complexity.

## Requirements

- MATLAB.
- Standard MATLAB numerical computing functions.

Additional toolbox requirements, if any, will be specified in the corresponding implementation files.

## How to Run

1. Download the MATLAB codes archive from this repository.
2. Extract the archive while preserving the directory structure.
3. Open MATLAB.
4. Navigate to the desired kernel directory.
5. Run the corresponding main MATLAB script.
6. Examine the generated numerical results, tables, and figures.

Detailed execution instructions and parameter settings will be provided with the individual implementations.

## Research Paper

**Title:** A Condition-Controlled Adaptive Direct RBF-PU Meshless Solver

**Authors:** Seyed Mehdi Mousavi, Mohsen Esmaeilbeigi, Gholamreza Garmanjani

**Affiliation:** Department of Mathematics, Faculty of Mathematical and Statistical Sciences, Malayer University, Malayer, Iran.

**Publication Status:** Manuscript submitted for peer review.

## Citation

If you use this repository in your research, please cite the corresponding publication:

Mousavi, S. M., Esmaeilbeigi, M., & Garmanjani, G., *A Condition-Controlled Adaptive Direct RBF-PU Meshless Solver*.

Publication details and DOI will be added after publication.

## Keywords

Direct RBF-PU; Radial Basis Functions; Partition of Unity; Adaptive Residual Subsampling; Hybrid Variably Scaled Kernels; Gaussian Kernel; Matérn Kernel; Thin Plate Spline; Elliptic Partial Differential Equations; Meshless Methods; Numerical Stability; Condition Number.
