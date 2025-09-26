# Modeling and Analysis of Synthetic Seismic Responses for Sleipner Simulation Models: a Case Study

**Autores:** Felipe L. Cavalcante<sup>1</sup>, Daiane Rossi Rosa Lessa<sup>1</sup>, Leonildes Soares de Melo Filho<sup>2</sup>, Denis José Schiozer<sup>1</sup>, Alessandra Davolio Gomes<sup>1</sup>       

<sup>1</sup> Center for Energy and Petroleum Studies, University of Campinas, Cora Coralina Street, 350, Campinas, SP, Brazil

<sup>2</sup> Repsol Sinopec Brasil - Praia de Botafogo, 300 – ZIP Code 22250-040, Rio de Janeiro, RJ – Brazil

Correspondence: felipeiag2012@gmail.com.br  

### Abstract
The Sleipner CO₂ storage project in the North Sea has become a global reference for carbon capture, utilization, and storage (CCUS), offering a dataset for testing geophysical methodologies. In this study, we assess the capacity of ten publicly available three-dimensional flow models from the British Geological Survey (BGS) to replicate observed four-dimensional seismic responses at the Sleipner East site. Real 4D seismic data provided by Equinor were compared against synthetic responses generated via petroelastic modeling and one-dimensional convolutional forward modeling of the simulation outputs. To address gaps in model documentation, we implemented a robust workflow that integrates literature-derived rock physics parameters with targeted calibration of petroelastic models. Model performance was quantified using the Structural Normalized Cross Correlation (NCC) and Root Mean Square Error (RMSE) metrics applied to attribute maps across three discrete reservoir intervals. Although none of the evaluated models capture every feature of the field data—reflecting their simplified geological frameworks—several closely reproduce the CO₂ plume morphology and signal polarity in specific zones. Our workflow enables reproducible seismic modeling for CCUS benchmarking, with Model 10 achieving the highest similarity (NCC = 0.754) in Zone 1. Moreover, this work provides a reproducible protocol for constructing petroelastic models and conducting seismic forward modeling using publicly accessible datasets for Sleipner.

## About
Repository containing a link to the synthetic data generated for the Sleipner case study.   

## Index

- [Repository Contents](#repository-contents)
- [Technical Specifications](#technical-specifications)
- [Instructions for Use](#instructions-for-use)
- [License](#license)

## Repository Contents   

This repository contains a link to files in SEG-Y. The files are stored in a public folder at https://drive.google.com/drive/folders/1aMspoNRo3P7fWS0vq47l9azuBc2lfu0U?usp=sharing

## Technical Specifications

The original files were generated using Schlumberger's Petrel software, with the Flow2Seis plugin installed. https://www.deepsoft.com.br/en/Projects/Flow2Seis

## Instructions for Use

Download the data and open the files in Schlumberger's Petrel software or another SEG-Y reader.

## License
All source code is made available under an MIT license. You can freely use and modify the code, without warranty, so long as you provide attribution to the authors. See 'LICENSE.md' for the full license text.

The manuscript text is not open source. The authors reserve the right to the article content, which is currently submitted for publication in the Geophysical Prospecting journal.
