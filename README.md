# Molecular-Similarity-Search-and-Clustering-Using-AI

This project performs molecular similarity analysis and clustering of chemical compounds using classical cheminformatics and machine learning techniques. It is designed to explore structural diversity in chemical datasets and support drug discovery efforts.

## Project Overview

The pipeline:

Generates Morgan fingerprints using RDKit

Calculates Tanimoto similarity between molecules

Clusters molecules using KMeans and Butina algorithms

Visualizes molecular clusters using UMAP


This approach provides insight into molecular diversity and similarity patterns without deep learning. FAISS is optional and can be used for faster similarity searches if desired.

## Tools & Libraries Used

Python

RDKit (fingerprints, similarity, clustering)

Pandas, NumPy (data handling)

Scikit-learn (KMeans clustering)

UMAP (visualization)

Matplotlib (plotting)


> Optional: FAISS can be used for fast similarity searches on large datasets.






## Workflow

1. Load molecular dataset in SMILES format


2. Generate Morgan fingerprints (radius=2, 1024 bits)


3. Compute Tanimoto similarity


4. Apply KMeans clustering (n_clusters=10)


5. Visualize clusters using UMAP


6. Apply Butina clustering for molecular grouping (distance threshold=0.4)


7. Save results as CSV files

Files Included

## File Name    	                   Description

molecular_similarity_project.ipynb	 Complete Jupyter Notebook with code & explanations

umap_clusters.png                  	 UMAP coordinates of molecules for cluster visualization
<img width="2400" height="1800" alt="umap_clusters" src="https://github.com/user-attachments/assets/9c652773-8247-4fab-805d-5ce28889eb44" />

Similarity_topk.csv	                 Top-k similar molecules using Tanimoto similarity

Butina_clusters_output.csv	          Butina clustering results with cluster IDs

Molecules_butina_clusters.csv	        Molecules mapped to their respective Butina clusters



## Key Results

Tanimoto Similarity

## Example similarity: ~0.115 → molecules are structurally very different

## Low similarity is good for exploring chemical diversity

## High similarity (>0.7) indicates potential analogs or scaffold similarity


## Clustering

KMeans: molecules grouped into 10 clusters

Butina: clusters formed using 0.4 distance threshold

Singleton clusters indicate high diversity, multi-molecule clusters indicate common scaffolds


## Visualization

UMAP plot shows spatial separation of clusters

Molecules with low Tanimoto similarity are far apart, reflecting diversity





## How to Run

1. Open molecular_similarity_project.ipynb in Jupyter Notebook or Google Colab


2. Run all cells sequentially


3. Outputs (CSV, UMAP plots) are automatically saved


4. Optional: Use FAISS for faster similarity searches on large dataset



## Author

## Sakshi Dhiman 💛

AI/ML in drug discovery and chemoinformatics

Experienced in molecular similarity analysis, clustering, and cheminformatics pipelines



   




