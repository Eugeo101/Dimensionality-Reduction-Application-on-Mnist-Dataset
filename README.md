# Dimensionality Reduction on MNIST-784 Dataset 📉  

This project focuses on applying dimensionality reduction techniques to the MNIST-784 dataset, improving model training efficiency, data compression, and data visualization.  

## 📝 Problem Statement  
High-dimensional datasets can be computationally expensive and hard to visualize. The goal of this project is to reduce the dimensionality of the MNIST-784 dataset while retaining important information, making it easier for machine learning models to train and visualize.  

## 🔍 Steps Followed:

### 1️⃣ Compression & Visualization  

#### a) Faster Training:
- Implemented PCA using two methods: **Eigenvalue-Vectors** and **SVD (Singular Value Decomposition)**.  
- Optimized the number of components using the **95% explained variance criterion** and **cumulative variance plot**, **also used n_components as a hyperparameter**.  
- Applied **IncrementalPCA** for handling large datasets efficiently, and used **Random Projection** when the number of features exceeded 20,000.

#### b) Data Compression:
- Reduced the dimensionality of the MNIST images using PCA and compared the **95% variance reconstructed images** with the original ones. This demonstrated the trade-off between **compression** and **information loss**.

#### c) Data Visualization:
- Used dimensionality reduction techniques to visualize high-dimensional data. Manifold Techniques used include:
  - **LLE (Locally Linear Embedding)**
  - **MDS (Multidimensional Scaling)**
  - **Isomap (Isometric Mapping)**
  - **t-SNE (t-Distributed Stochastic Neighbor Embedding)**
  
- Specifically, applied **t-SNE** to visualize the reduced feature space of the MNIST digits dataset, capturing the underlying structure of the data in 2D. This helped in identifying clusters and patterns in the data.

### 2️⃣ Performance and Results  
- Achieved significant dimensionality reduction, improving training speed without losing crucial data information.  
- Successfully demonstrated compression benefits with minimal image distortion.  
- Visualized the MNIST dataset using **t-SNE**, revealing the underlying structure of handwritten digits.  

### 3️⃣ Conclusion  
- Applied PCA and t-SNE for dimensionality reduction, demonstrating improvements in training, compression, and visualization of high-dimensional data.  
