# Soil Analysis using KMeans Clustering

## Project Overview
This project analyzes soil nutrient data, specifically focusing on Nitrogen levels and pH values, using KMeans clustering to identify patterns and groupings in soil samples. The analysis aims to guide lime application and fertilizer optimization strategies for improved soil health and sustainability.

## Author
- Name: Albright Maduka Ifechukwude
- Student ID: 9053136
- Course: PROG8431 - Data Analysis Mathematics and Algorithm Model

## Features
- Data cleaning and preprocessing of soil nutrient data
- Feature scaling using StandardScaler
- Optimal cluster determination using both Elbow Method and Silhouette Score
- KMeans clustering implementation
- Visualization of cluster distributions and results
- Statistical summary of cluster characteristics

## Project Structure
```
ClusteringKMeans_Workshop/
├── ClusteringKMeans_Workshop.ipynb   # Main Jupyter notebook
├── Data/
│   └── Soil Nutrients.csv            # Input data
├── Clustered_Soil_Data.csv          # Output: Processed data with cluster assignments
└── Cluster_Centers.csv              # Output: Final cluster centroids
```

## Technical Requirements
- Python 3.x
- Required Libraries:
  - numpy
  - pandas
  - matplotlib
  - scikit-learn

## Methodology
1. Data Loading and Preprocessing
   - Load soil nutrient data
   - Clean and filter data based on N and pH bounds
   - Scale features for clustering

2. Clustering Analysis
   - Determine optimal number of clusters (k) using:
     - Elbow Method
     - Silhouette Score
   - Apply KMeans clustering
   - Visualize results and cluster distributions

3. Results Analysis
   - Generate cluster summaries with statistical measures
   - Save processed data and cluster centers for reproducibility

## Output Files
- `Clustered_Soil_Data.csv`: Contains the original data with cluster assignments
- `Cluster_Centers.csv`: Contains the coordinates of cluster centroids in original units

## Usage
Open and run the Jupyter notebook `ClusteringKMeans_Workshop.ipynb` to:
1. Load and preprocess the soil data
2. Perform clustering analysis
3. Visualize results
4. Generate output files