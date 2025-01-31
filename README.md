# Neural-Network-for-Diagnosis-of-Retinal-Diseases
This document is part of my coursework, where I review the paper "Optic-Net: A Novel Convolutional Neural Network for Diagnosis of Retinal Diseases from Optical Tomography Images" and attempt to replicate its experiments. The paper was published by Sharif Amit Kamran, Sourajit Saha, Ali Shihab Sabbir, and Alireza Tavakkoli in 2019 and proposes a novel CNN architecture, Optic-Net, designed to diagnose retinal diseases from Spectral Domain Optical Coherence Tomography (SD-OCT) images.

## Overview
This repository contains the implementation of **Optic-Net**, a novel Convolutional Neural Network (CNN) architecture designed for the diagnosis of retinal diseases from Spectral Domain Optical Coherence Tomography (SD-OCT) images. The model achieves state-of-the-art performance with near-perfect accuracy on two separate datasets: **OCT2017** and **Srinivasan2014**.

The paper, titled **"Optic-Net: A Novel Convolutional Neural Network for Diagnosis of Retinal Diseases from Optical Tomography Images"**, was published by Sharif Amit Kamran, Sourajit Saha, Ali Shihab Sabbir, and Alireza Tavakkoli in 2019. The paper proposes a new CNN architecture that addresses issues like gradient explosion and degradation, achieving 99.8% accuracy on the OCT2017 dataset and 100% accuracy on the Srinivasan2014 dataset.

## Key Features
- **Novel CNN Architecture**: The proposed architecture introduces:
  - A new residual unit incorporating **Atrous Separable Convolution**.
  - A new building block for better feature extraction.
  - A mechanism to prevent gradient degradation.
- **High Accuracy**: Achieves near-perfect accuracy on retinal disease classification.
- **Efficient Training**: The model is optimized to handle large datasets efficiently.

## Datasets
The model was trained and tested on two publicly available datasets:
1. **OCT2017**: Contains thousands of validated OCT images labeled into four categories: CNV, DME, DRUSEN, and NORMAL.
2. **Srinivasan2014**: Contains volumetric scans from 45 patients, labeled as NORMAL, DME, and AMD.

## Code Structure
The repository is organized as follows:
- **dataloader.py**: Contains functions to load and preprocess the OCT2017 and Srinivasan2014 datasets.
- **metrics.py**: Includes functions to compute evaluation metrics such as accuracy, specificity, and sensitivity.
- **model.py**: Implements the Optic-Net CNN architecture.
- **train.py**: Script to train the model on the selected dataset.
- **test.py**: Script to test the trained model on new data.
- **visualize.py**: Functions to plot training and validation loss/accuracy.

## Results
The model achieves the following results:
- OCT2017 Dataset: 99.8% accuracy.
- Srinivasan2014 Dataset: 100% accuracy.

## References
- Kamran, S. A., Saha, S., Sabbir, A. S., & Tavakkoli, A. (2019). Optic-Net: A Novel Convolutional Neural Network for Diagnosis of Retinal Diseases from Optical Tomography Images. arXiv preprint arXiv:1910.05672.
- Kermany, D. S., et al. (2018). Identifying Medical Diagnoses and Treatable Diseases by Image-Based Deep Learning. Cell, 172(5), 1122-1131.
- Srinivasan, P. P., et al. (2014). Fully automated detection of diabetic macular edema and dry age-related macular degeneration from optical coherence tomography images. Biomedical Optics Express, 5(10), 3568-3577.
