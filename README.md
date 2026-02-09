# PCA_AfricaMalaria_formative2

# Project Overview
This project implements Principal Component Analysis (PCA) from scratch using Python (NumPy) without relying on high-level libraries like sklearn for the core algorithms. The goal is to reduce the dimensionality of a high-dimensional African Malaria dataset while preserving the maximum variance/information.

The project demonstrates:
- Data cleaning and handling of real-world "messy" data (missing values, categorical features).
- Mathematical implementation of Covariance, Eigenvalues, and Eigenvectors.
- Dimensionality reduction from 27 dimensions down to 2 dimensions.
- Visualization of the African dataset before and after PCA.

# The Dataset
Name: DatasetAfricaMalaria.csv  
Source: Kaggle
Description: This impactful dataset tracks malaria incidence and related factors across 54 African nations.
- Original Dimensions: 27 columns (including Incidence of malaria, Bed net use, Sanitation, Rural/Urban population, etc.).
- Challenges: Contains significant missing data (NaN) and non-numeric columns (Country Name, Country Code), requiring robust preprocessing.

# Tech Stack
* Python 3.x
* NumPy: For linear algebra operations (matrix multiplication, eigendecomposition).
* Pandas: For data loading and cleaning.
* Matplotlib: For visualization (scatter plots).

# Installation & Usage
1.  Clone the repository:
    ```bash
    git clone [https://github.com/YOUR_USERNAME/alu-advanced-linear-algebra-pca.git](https://github.com/YOUR_USERNAME/alu-advanced-linear-algebra-pca.git)
    cd alu-advanced-linear-algebra-pca
    ```

2.  Install dependencies:**
    ```bash
    pip install numpy pandas matplotlib seaborn
    ```

3.  Run the Notebook:
    Open the Jupyter Notebook (.ipynb file) in Google Colab or Jupyter Lab and run all cells sequentially.

# Methodology (Steps Performed)
1.  Data Cleaning: Loaded the raw African Malaria data. Handled non-numeric columns (Country Name) and imputed missing values using column means.
2.  Standardization: Applied the Z-score formula $z = \frac{x - \mu}{\sigma}$ to normalize features with different scales (e.g., population vs. percentages).
3.  Covariance Matrix: Calculated the covariance matrix to understand relationships between the 27 variables.
4.  Eigendecomposition: Computed Eigenvalues and Eigenvectors to identify the principal components.
5.  Sorting: Ranked components by explained variance (High to Low).
6.  Projection: Projected the 27D data onto the top 2 Principal Components (2D).
7.  Visualization: Plotted the projected data to reveal clusters and structure.

# Results
* Dimensionality Reduction: Successfully reduced data from 27 dimensions to 2.
* Visualization: The final scatter plot visualizes the spread of African countries based on their health and demographic profiles.
* Variance Explained: The script calculates the exact percentage of information retained by the top components.

# Author
Larissa Iriza 
