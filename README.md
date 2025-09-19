# Modeling and Analysis of Synthetic Seismic Responses for Sleipner Simulation Models: A Case Study

**Autores:** Felipe L. Cavalcante<sup>1</sup>, Daiane Rossi Rosa Lessa<sup>1</sup>, Denis José Schiozer<sup>1</sup>, Alessandra Davolio Gomes<sup>1</sup>       

<sup>1</sup> Center for Energy and Petroleum Studies, University of Campinas, Cora Coralina Street, 350, Campinas, SP, Brazil  

Correspondence: felipeiag2012@gmail.com.br  

### Abstract
The Sleipner CO₂ storage project in the North Sea has become a global reference for carbon capture, utilization, and storage (CCUS), offering an unparalleled dataset for testing geophysical methodologies. In this study, we assess the capacity of ten publicly available three-dimensional flow models from the British Geological Survey (BGS) to replicate observed four-dimensional seismic responses at the Sleipner East site. Real 4D seismic data provided by Equinor were compared against synthetic responses generated via petroelastic modeling and one-dimensional convolutional forward modeling of the simulation outputs. To address gaps in model documentation, we implemented a robust workflow that integrates literature-derived rock physics parameters with targeted calibration of petroelastic models. Model performance was quantified using the Structural Normalized Cross Correlation (NCC) and Root Mean Square Error (RMSE) metrics applied to attribute maps across three discrete reservoir intervals. Although none of the evaluated models capture every feature of the field data—reflecting their simplified geological frameworks—several closely reproduce the CO₂ plume morphology and signal polarity in specific regions. Moreover, this work provides a reproducible protocol for constructing petroelastic models and conducting seismic forward modeling using publicly accessible datasets for Sleipner.

## About
Repository containing scripts for 2D magnetic forward modeling and inversion of thin dikes.   

## Index

- [Repository Contents](#repository-contents)
- [Folder Structure](#folder-structure)
- [Technical Specifications](#technical-specifications)
- [Instructions for Use](#instructions-for-use)
- [License](#license)

## Repository Contents   

This repository contains the files necessary to reproduce the results obtained in this research. The content is organized into folders that contain:

- **Scripts:** used for forward modeling, processing, inversion, and data analysis.

## Folder Structure

The organization of this repository follows the structure below:

```plaintext
Minerals_IMADS/
├── README.md                    # This file
├── LICENSE.md                   # License file
├── PyDyke_env.yml               # Virtual environment configuration file
├── Data/ (real and synthetic data)
├── FWD/ (folder of the forward problem)
│   ├── Input/
│   │   └── (input files for running the forward problem)
│   ├── Output/
│   │   └── (output files from the forward problem)
│   ├── 1_PyDyke_Extent_n_Disturb.py (file for executing the forward problem)
│   ├── 2_PyDyke_cut_data.py (file for cropping the data)
│   ├── func_*.py (files containing functions for executing the forward problem)
├── INV/ (folder of the inverse problem)
│   ├── Input/
│   │   └── (input files for running the inverse problem)
│   ├── Output/
│   │   └── (output files from the inverse problem)
│   ├── 1_PyDyke_simple_filt.py (file for filtering data)
│   ├── 2_PyDyke_d2T.py (file for calculating the second derivative of the data)
│   ├── 3_PyDyke_lims.py (file for setting model limits)
│   ├── 4_PyDyke_calc_initial.py (file for calculating the initial solution for the problem)
│   ├── 5_PyDyke_inv.py (file for executing the inverse problem)
│   ├── 6_PyDyke_plot.py (file for plotting the results of the inverse problem)
│   ├── 7_PyDyke_STD.py (file for calculating and plotting the standard deviation of the solutions)
│   ├── 8_PyDyke_join_exit_std.py (file for compiling solutions and probabilities into a table)
│   ├── func_*.py (files containing functions for executing the inverse problem)
```


## Technical Specifications

The original files were generated using Schlumberger's Petrel software, with the Flow2Seis plugin installed.

## Instructions for Use

Download the data and open the files in Schlumberger's Petrel software or another SEG-Y reader.

## License
All source code is made available under an MIT license. You can freely use and modify the code, without warranty, so long as you provide attribution to the authors. See 'LICENSE.md' for the full license text.

The manuscript text is not open source. The authors reserve the right to the article content, which is currently submitted for publication in the Geophysical Prospecting.
