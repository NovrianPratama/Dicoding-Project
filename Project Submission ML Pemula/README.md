# Bank Marketing Campaign: Clustering and Classification Analysis 🚀

This repository contains an end-to-end project focused on analyzing bank marketing campaign data. By leveraging clustering and classification techniques, we aim to uncover customer insights and optimize campaign strategies.

## 📊 Project Overview
- **Dataset 1:** `bank.csv` – Raw data used for clustering to group customers based on their demographic and behavioral attributes.
- **Dataset 2:** `bank_campaign.csv` – Enhanced dataset with cluster labels, used for training classification models.

## 🧠 Key Highlights
1. **Clustering Analysis:**
   - KMeans clustering identified three distinct customer groups (Cluster 0, 1, 2) with unique profiles:
     - **Cluster 0:** White-collar professionals active in Q2, yet with low campaign success rates.
     - **Cluster 1:** Service workers active in Q3, needing focused offers.
     - **Cluster 2:** Professionals with more consistent activity throughout the year.
   - Insights provided actionable strategies to target campaigns more effectively.

2. **Classification Analysis:**
   - **Decision Tree:** Achieved 100% accuracy but exhibited overfitting, indicating a need for improved tuning.
   - **Random Forest:** Post-tuning, achieved 99.92% accuracy with better generalization.
   - **SMOTE Handling:** Addressed class imbalance effectively during training.

## 🛠️ Technologies Used
- **Python:** Pandas, NumPy, Matplotlib/Seaborn for data analysis and visualization.
- **Machine Learning:** Scikit-learn for clustering and classification.
- **SMOTE:** Handled class imbalance during model training.

## 🌟 Results and Recommendations
- Targeted campaign strategies tailored to customer clusters.
- Suggestions for improving classification models through advanced techniques like Gradient Boosting.

## 🚀 Future Improvements
- Extend dataset with new features to improve clustering and classification accuracy.
- Explore additional models like XGBoost or LightGBM to address overfitting.

Thank you for visiting! 😊
