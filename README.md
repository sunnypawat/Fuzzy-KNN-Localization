# Fuzzy-KNN Weighted Centroid Localization (FKWCL)

**Authors:** Pawat Songkhopanit and Mariia Afonina

## Overview

This repository contains the implementation and simulation environment for the **Fuzzy-KNN Weighted Centroid Localization (FKWCL)** algorithm, a novel, lightweight method designed to improve location estimation accuracy and robustness in Wireless Sensor Networks (WSN) and IoT environments.

The FKWCL algorithm enhances traditional Weighted Centroid Localization (WCL) by incorporating two key features:

1.  **K-Nearest Neighbor (KNN) Anchor Selection:** Selects anchors not just by distance but also by **angular diversity** to mitigate geometric bias.
2.  **Fuzzy Weighting:** A sophisticated weighting function that combines both **distance-closeness** and **angular-separation** to reduce errors, particularly in non-uniform anchor layouts.

This work addresses the critical need for geometry-aware localization in resource-constrained range-free networks.

## Repository Structure

* `project.ipynb`: The main Jupyter Notebook containing the Python implementation of Centroid, WCL, and FKWCL algorithms, the simulation environment setup, and the performance evaluation against varying anchor layouts, anchor densities, and radio irregularity (DOI).
* `report_KNN_FKWCL.pdf`: The complete research paper ("Centroid vs WCL vs Fuzzy-KNN-WCL: Simulation and Performance Evaluation") detailing the methodology, mathematical model, simulation setup, and comprehensive results.

## Key Features and Performance

The simulations demonstrate that FKWCL significantly outperforms Centroid and standard WCL, especially in challenging environments.

| Metric | FKWCL Improvement over Centroid | FKWCL Improvement over WCL |
| :--- | :--- | :--- |
| **Localization Error** (Mean Reduction) | Up to **75%** | **20–40%** |
| **Geometric Bias Reduction** (L-shape layout) | $\approx 45\%$ | $\approx 22\%$ |
| **Computational Cost** | Minimal overhead (microsecond-level runtime) | Minimal overhead |

### Visualization of FKWCL's Robustness


## Requirements

To run the simulations in the `project.ipynb` notebook, you will need a standard Python data science environment.

1.  **Python 3.x**
2.  **Jupyter Notebook** or **JupyterLab**
3.  The following Python libraries:
    * `numpy`
    * `pandas`
    * `scipy`
    * `matplotlib` (for plotting results)

You can install the necessary dependencies using `pip`:

```bash
pip install numpy pandas scipy matplotlib jupyter
