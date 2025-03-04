# Course Platform User Consumption Behavior Analysis

## Overview
This project aims to analyze user consumption behavior on an online course platform. The goal is to identify high-value users and optimize marketing costs by leveraging data-driven insights. We utilize various data processing, visualization, feature engineering, and modeling techniques to predict user purchasing behavior and provide actionable recommendations for business growth.


## Project Structure

### 1. Problem Statement
With the growing influence of the internet, companies are continuously seeking effective online customer acquisition strategies. One major challenge is identifying high-quality users and channels while minimizing marketing costs. By analyzing user behavior data, we can evaluate user value and implement targeted marketing strategies to enhance conversion rates.

### 2. Data Preprocessing & Feature Engineering
- **Data Sources:**
  - `user_info.csv`: Contains user demographic information.
  - `login_day.csv`: Logs user login activity.
  - `visit_info.csv`: Records user visits and interactions.
  - `result.csv`: Tracks user purchase history.
- **Preprocessing Steps:**
  - Handling missing values, erroneous data, and anomalies.
  - Converting data types (e.g., date formatting, age conversion).
  - Feature engineering including encoding categorical features, deriving new temporal features, and standardizing numerical features.

### 3. Data Visualization
- Analyzed city-wise user distribution and login trends.
- Created various visual representations of data insights to enhance understanding.

### 4. Model Analysis
Implemented multiple machine learning models to predict whether users would place an order:
- **Logistic Regression (LR)**: Applied PCA for dimensionality reduction and analyzed recall values.
- **LightGBM**: Optimized using grid search, adjusting depth, leaf nodes, and learning rate to improve recall.
- **Random Forest**: Tuned hyperparameters to enhance F1 score and recall.
- **Backpropagation Neural Network (BP)**: Optimized using stochastic gradient descent (SGD) and adjusted learning rate to enhance performance.

### 5. User Consumption Behavior Value Analysis
- **RFEM Model:** Combined RFE and RFM models to determine the impact of features on user purchasing behavior.
- **K-Means Clustering:** Identified four user groups based on consumption behavior:
  - **Core Value Users** (High engagement & purchase rate)
  - **Important Value Users** (High login frequency but low engagement)
  - **Potential Value Users** (Recent activity increase, low historical engagement)
  - **Low-Value Users** (Minimal engagement and low purchase history)
- **Marketing Strategies:**
  - Maintain strong relationships with core users.
  - Encourage engagement from important value users.
  - Identify and nurture potential value users.
  - Minimize investment in low-value users.

## Key Results
- Successfully identified user segments based on purchasing behavior.
- Achieved a prediction model accuracy of over 85%.
- Provided data-driven marketing recommendations to enhance customer engagement and optimize costs.

## Future Work
- Expand analysis to incorporate external factors influencing user engagement.
- Enhance model performance with deep learning approaches.
- Implement real-time analytics for dynamic marketing strategies.

## How to Use This Repository
1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd <repository_name>
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the data preprocessing script:
   ```bash
   python preprocess.py
   ```
4. Train and evaluate models:
   ```bash
   python train.py
   ```
5. View visualizations and insights:
   ```bash
   python visualize.py
   ```

## Acknowledgments
This project was completed as part of a data analysis course, with contributions from all team members. We appreciate the guidance from our instructors and peers.
