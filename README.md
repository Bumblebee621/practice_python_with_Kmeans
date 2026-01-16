# K-Means Clustering & London Bike Sharing Analysis

## Overview
This project implements the **K-Means clustering algorithm from scratch** using NumPy and applies it to analyze the London Bike Sharing dataset. It demonstrates a complete data science workflow: from data cleaning and feature engineering to statistical analysis and unsupervised learning.

The goal is to identify patterns in bike sharing usage (`cnt`) based on temperature (`t1`) and other environmental factors.

## Key Features
*   **K-Means Implementation:** A custom implementation of the K-Means algorithm, including random centroid initialization, cluster assignment, and centroid recomputation.
*   **Data Engineering:** comprehensive preprocessing pipeline using **Pandas**:
    *   Timestamp parsing and extraction of temporal features (Hour, Day, Month, Year).
    *   Categorical mapping (Seasons) and creation of composite features (e.g., `is_weekend_holiday`).
    *   Feature scaling (Min-Max normalization) and noise injection for robustness.
*   **Statistical Analysis:** Automated generation of descriptive statistics and correlation matrices to identify relationships between variables (e.g., temperature vs. "feels like" temperature).
*   **Visualization:** Dynamic scatter plots using **Matplotlib** to visualize clusters and centroids for different values of $k$.

## Technologies
*   **Python 3.x**
*   **NumPy:** Vectorized operations for efficient distance calculations and matrix manipulations.
*   **Pandas:** Data manipulation, cleaning, and aggregation.
*   **Matplotlib:** Data visualization.

## Project Structure
*   `main.py`: Entry point. Orchestrates the data loading, analysis (Part A), and clustering execution (Part B).
*   `clustering.py`: Contains the core logic for the K-Means algorithm, data transformation, and visualization functions.
*   `data.py`: Handles data loading, cleaning, feature extraction, and exploratory data analysis (EDA).
*   `london.csv`: Input dataset containing historical bike sharing and weather data.

## Getting Started

1.  **Clone the repository**
2.  **Install dependencies:**
    ```bash
    pip install numpy pandas matplotlib
    ```
3.  **Run the analysis:**
    ```bash
    python main.py
    ```

## Results
The program outputs statistical insights to the console and saves clustering visualizations (e.g., `results_k3.png`) showing how bike usage groups under different conditions.

---
*Created by Ariel Assis as a demonstration of Python programming and Machine Learning fundamentals.*
