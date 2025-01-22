# Bank Marketing Campaign: Clustering and Classification Analysis 🚀

Welcome to the repository for analyzing and optimizing bank marketing campaigns using clustering and classification techniques. This project aims to gain insights into customer behavior and improve marketing strategies by leveraging machine learning and data analysis.

## 🔍 Project Objectives

- **Customer Segmentation**: Perform customer segmentation using clustering techniques to identify distinct customer groups.
- **Classification Models**: Train and evaluate classification models to predict customer responses to marketing campaigns.
- **Campaign Optimization**: Provide actionable insights to optimize campaign strategies and improve overall success rates.

## 📈 Datasets

1. **bank.csv (Raw Data)**:
   - **Purpose**: Used for clustering analysis to group customers based on demographic and behavioral attributes.
   - **Key Features**:  
     - `age`, `job`, `marital`, `education`, `balance`, `housing`, `loan`, etc.  
     - **Target variable**: `deposit` (Yes/No indicating if a customer subscribed to a term deposit).

2. **bank_campaign.csv (Processed Data)**:
   - **Purpose**: Enhanced dataset with cluster labels for classification analysis.
   - **Key Features**:  
     - Includes binned categorical variables such as `job_binned`, `month_binned`, and numeric variables like `balance_binned`.  
     - **Cluster labels** (`KMeans_Cluster`) added as target variables for classification.

## 🔦 Key Analyses and Results

### Clustering Analysis

Using **KMeans** clustering, customers were segmented into three distinct groups:

#### ✨ Cluster 0:
- **Size**: 2771 customers.
- **Key Characteristics**:
  - Dominated by white-collar professionals (`job_binned_white-collar mean: 0.5699`).
  - Most active in **Q2** (`month_binned_Q2 mean: 0.6996`).
  - Low success in past campaigns (`poutcome_binned_other mean: 0.9972`).
  - **Balance**: Low to medium.
  - Majority are **married** (`marital_married mean: 0.565`).

#### ✨ Cluster 1:
- **Size**: 1532 customers.
- **Key Characteristics**:
  - Focus on **service jobs** (`job_binned_services mean: 0.0954`).
  - Higher activity in **Q3** (`month_binned_Q3 mean: 0.1151`).
  - **Balance**: Mostly low.
  - **Education**: Predominantly secondary.

#### ✨ Cluster 2:
- **Size**: 2254 customers.
- **Key Characteristics**:
  - Similar to **Cluster 0** but with more consistent activity throughout the year.
  - **Balance**: Low to medium.
  - Higher proportion of **tertiary education** compared to other clusters.

### Classification Analysis

**Models Used**:
- **Decision Tree**:
  - **Before Tuning**: Achieved 100% accuracy, indicating overfitting.
  - **After Tuning**: Accuracy remained high but overfitting persisted.
  - **Issue**: Model complexity not well-regularized.

- **Random Forest**:
  - **Before Tuning**: Accuracy was 100%, suggesting potential overfitting.
  - **After Tuning**: Accuracy adjusted to 99.92%, showing better generalization.
  - **Strength**: Handled class imbalance effectively with **SMOTE**.

**Key Metrics**:
- **Accuracy**: High across both models, but **Random Forest** exhibited better performance after tuning.
- **Overfitting** was addressed with **hyperparameter tuning** and **feature engineering**.

## 🛠️ Technologies and Tools

- **Programming Language**: Python
- **Libraries**:  
  - Data Analysis: Pandas, NumPy  
  - Visualization: Matplotlib, Seaborn  
  - Machine Learning: Scikit-learn, SMOTE
- **Algorithms**:  
  - Clustering: KMeans  
  - Classification: Decision Tree, Random Forest

## 💡 Insights and Recommendations

- **Targeted Campaigns**:
  - **Cluster 0**: Focus on campaigns in **Q2** with personalized offers for professionals.
  - **Cluster 1**: Emphasize campaigns in **Q3** with relevant offers for service workers.
  - **Cluster 2**: Maintain consistent campaigns throughout the year with high-quality offerings.

- **Model Improvements**:
  - Experiment with **Gradient Boosting** techniques (XGBoost, LightGBM).
  - Use more diverse data to enhance model generalizability.

- **Feature Engineering**:
  - Create additional features to capture more nuanced customer behavior.
  - Refine binning strategies for categorical variables
 
## 🎨 Future Work

- Incorporate additional datasets to capture external factors influencing customer behavior.
- Explore advanced clustering methods (e.g., **DBSCAN**) to handle outliers.
- Implement **deep learning models** for further classification improvements.

## 📢 Contribute

Contributions are welcome! Feel free to fork this repository, open issues, or submit pull requests to improve this project. Together, we can optimize marketing strategies for better outcomes.

## 📊 Acknowledgments

Special thanks to the data science community for their continuous support and inspiration.


Thank you for visiting! 😊
