# gReLU-Inference-to-Predict-RNA-seq-Coverage
This project uses the Borzoi model from gReLU to predict RNA-seq coverage tracks given a DNA genomic sequence. gReLU is a Python library to train, interpret, and apply deep learning models to DNA sequences. Borzoi is one of the pre-trained models from the model zoo that uses a convolutional neural network to predict RNA-seq coverage given 524kb input sequences. 

## Table of Contents
- [Background](#background)
- [Borzoi Architecture](#Borzoi-Architecture)
- [Model Performance](#Model-Performance)
- [In-Silico Mutagenesis](#In-Silico-Mutagenesis)
   - [Heatmap](#Heatmap)
   - [Sequence Logo Map](#Sequence-Logo-Map)
- [Citations](#Citations) 

--- 

## Background


## Borzoi Architecture 

The Borzoi architecture consists of a U-net with a tower of convolution- and subsampling blocks followed by a series of self-attention blocks operating at 128 bp resolution
embedding vectors in the contracting path. Self-attention is a critical feature of this model as it allows every pair of position vectors to exchange information. In the expansive path the 
vectors are upsampled from the attention blocks and combined with the corresponding feature map of equal size produced by the initial convolution tower. 

![Borzoi Architecture](Images/Borzoi-Architecture.png) 

## Model Performance 


## In-Silico Mutagenesis 


### Heatmap 


### Sequence Logo Map 

---
## Citations 
**Paper Citation**: Linder, J., Srivastava, D., Yuan, H., Agarwal, V., & Kelley, D. R. (2023). Predicting RNA-seq coverage from DNA sequence as a unifying model of gene regulation. bioRxiv. https://doi.org/10.1101/2023.08.30.555582

**Code adopted from**: https://github.com/Genentech/gReLU/tree/main

Any comments, questions, or suggestions are greatly appreciated! Thank you. 
