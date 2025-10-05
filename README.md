# Assignment 5 - Visualizing Data Veracity Challenges in Multi-label Classification

## Author
Name : G C V Sairam  
Roll No : DA25M012  
Department : M.Tech, Data Science and Artificial Intelligence  


## Overview
This assignment explores data veracity challenges in the Yeast Dataset using manifold learning techniques. The dataset contains gene expression features and 14 functional category labels, exhibiting issues like noisy labels, outliers, and ambiguous classification regions.

## Dataset
- **Source**: Yeast Dataset (yeast.arff)
- **Samples**: 2,417 experiments
- **Features**: 103 gene expression levels
- **Labels**: 14 binary functional categories

## Key Objectives
1. Apply dimensionality reduction techniques (t-SNE and Isomap) to visualize high-dimensional gene expression data
2. Identify and examine data quality issues including:
   - Noisy/ambiguous labels
   - Outliers
   - Mixed functional category regions
3. Understand classification challenges through visual inspection

## Methodology

### Data Preprocessing
- Load and parse ARFF format data
- Convert label columns to numeric values
- Standardize features for distance-based techniques
- Identify visualization categories:
  - Two most frequent single-label classes
  - Most frequent multi-label combination
  - "Other" category for remaining instances

### Manifold Learning Techniques
1. **t-SNE (t-Distributed Stochastic Neighbor Embedding)**
   - Preserves local structure and reveals cluster patterns
   - Perplexity parameter optimization (5-50 range)

2. **Isomap (Isometric Mapping)**
   - Preserves geodesic distances
   - Captures global data structure

## Implementation
The notebook includes:
- Data loading and preprocessing pipelines
- Feature scaling using StandardScaler
- t-SNE and Isomap implementations
- Visualization of 2D embeddings colored by label categories
- Analysis of data veracity challenges
