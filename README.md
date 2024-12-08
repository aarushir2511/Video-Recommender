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


## Usage
-**Step 1: Prepare Data**

Place unified_interactions.csv and final_all_posts_df.csv in the data/ directory.

-**Step 2: Run the Script**

Execute the main script to calculate evaluation metrics:

Example Output
  ```bash
    Content-Based MAE: 0.24, RMSE: 0.31
    Collaborative Filtering MAE: 0.30, RMSE: 0.37
    Hybrid MAE: 0.22, RMSE: 0.29
  ```

## Code Highlights
# Evaluation Logic

The [calculate_metrics] function evaluates each recommendation model:

```bash
Python
from sklearn.metrics import mean_absolute_error, mean_squared_error

def calculate_metrics(actual_ratings, predicted_ratings):
    mae = mean_absolute_error(actual_ratings, predicted_ratings)
    rmse = np.sqrt(mean_squared_error(actual_ratings, predicted_ratings))
    return mae, rmse
```


## License
This project is licensed under the MIT License. See the LICENSE file for details.   

## Contact
Author: [Aarushi Ranjan]
Email: [aarushiranjan0@example.com]
