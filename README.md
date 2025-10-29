# Soil Analysis using KMeans Clustering

## Project Overview
This project analyzes soil nutrient data, specifically focusing on Nitrogen levels and pH values, using KMeans clustering to identify patterns and groupings in soil samples. The analysis reveals relationships between nitrogen content and soil acidity, helping identify regions that may require lime application or adjusted fertilization strategies. These insights contribute to improved soil health management and sustainable agricultural practices.

## Project Context
- **Domain**: Canada Agriculture
- **Focus**: Nitrogen vs Soil pH Analysis
- **Goal**: Identify soil management zones through clustering analysis

## Author
- Name: Albright Maduka Ifechukwude
- Student ID: 9053136
- Course: PROG8431 - Data Analysis Mathematics and Algorithm Model

## Key Findings
The K-means analysis identified three distinct soil clusters:
1. **Low-N/Near-Neutral**: ~45 N, 6.9 pH - Stable soils with balanced conditions
2. **Moderate-N/Slightly-Acidic**: ~95 N, 6.2 pH - Transition zone requiring monitoring
3. **High-N/More-Acidic**: ~140 N, 5.7 pH - Areas requiring potential lime application

These clusters provide valuable insights for:
- Targeted lime application in acidic zones
- Optimized nitrogen fertilization strategies
- Identification of stable soil regions

## Features
- Automated detection and extraction of Nitrogen and pH columns
- Robust data cleaning with configurable bounds for N (0-200) and pH (2.5-9.5)
- Feature standardization using StandardScaler
- Optimal cluster determination using:
  - Elbow Method for variance explanation
  - Silhouette Score for cluster quality
- Interactive visualizations:
  - Feature distributions (histograms and boxplots)
  - Cluster scatter plots with centroids
  - Model selection curves
- Comprehensive statistical summaries:
  - Per-cluster statistics (mean, min, max)
  - Sample counts per cluster
  - Centroid coordinates in original units

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
   - Automated loading and column detection
   - Smart cleaning with regex-based numeric conversion
   - Outlier removal using configurable bounds
   - Feature standardization for unbiased clustering

2. Model Selection
   - Systematic evaluation of k values (2-6)
   - Dual criteria approach:
     - Elbow Method: Assesses variance explanation
     - Silhouette Score: Measures cluster quality
   - Automated selection of optimal k

3. Clustering Analysis
   - K-means implementation with multiple initializations
   - Standardized space clustering
   - Back-transformation to original units
   - Comprehensive visualization suite

4. Results Interpretation
   - Statistical profiling of clusters
   - Identification of management zones
   - Agricultural implications analysis
   - Export of reproducible results

## Output Files
- `Clustered_Soil_Data.csv`: Contains the original data with cluster assignments
- `Cluster_Centers.csv`: Contains the coordinates of cluster centroids in original units

## Usage
Open and run the Jupyter notebook `ClusteringKMeans_Workshop.ipynb` to:
1. Load and preprocess the soil data
2. Perform clustering analysis
3. Visualize results
4. Generate output files