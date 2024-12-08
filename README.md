# Recommendation System Evaluation Framework

## Overview
This project evaluates three types of recommendation systems:  
- **Content-Based Filtering**
- **Collaborative Filtering**
- **Hybrid Recommendations**

It uses metrics like **Mean Absolute Error (MAE)** and **Root Mean Square Error (RMSE)** to assess the performance of the recommendations.

---

## Features
- **Content-Based Filtering**: Recommends posts based on similarity scores from post attributes.
- **Collaborative Filtering**: Uses user-item interactions and similarity matrices for recommendations.
- **Hybrid Recommendations**: Combines content-based and collaborative methods for enhanced performance.
- **Evaluation Metrics**:
  - **MAE**: Measures the average error magnitude.
  - **RMSE**: Considers error magnitude with variance.

---

## Technologies Used
- **Programming Language**: Python
- **Libraries**:
  - `scikit-learn`: For evaluation metrics like MAE and RMSE.
  - `pandas`, `numpy`: For data manipulation and numerical computations.

---

## Project Structure
├── data/ │ ├── unified_interactions.csv # User-post interactions dataset │ ├── final_all_posts_df.csv # Posts metadata and similarity scores ├── recommenders/ │ ├── content_based.py # Content-based recommendation logic │ ├── collaborative.py # Collaborative filtering logic │ ├── hybrid.py # Hybrid recommendation logic ├── evaluation/ │ ├── metrics.py # Evaluation metrics logic │ ├── evaluate.py # Scripts for model evaluation ├── README.md # Project documentation └── main.py # Main script for execution

