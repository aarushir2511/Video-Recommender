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

## Dataset
- **Unified Interactions**: Contains `user_id`, `post_id`, `viewed_at`, `liked_at`, `inspired_at` and `rating_percent`.
- **Posts Metadata**: Contains `post_id` and attributes for calculating similarity scores.

---

## Installation

### Prerequisites
1. Python 3.8+
2. Required Python libraries:
   ```bash
   pip install pandas numpy scikit-learn


