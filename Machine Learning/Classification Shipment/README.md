# E-Commerce Customer Shipment Classification 📦🕒


This project focuses on predicting whether products will reach their destination on time using multiple **Machine Learning Classification** algorithms. We evaluate models like **Decision Tree**, **Naive Bayes**, **K-Nearest Neighbours (KNN)**, **Random Forest**, and **Support Vector Machine (SVM)** using the **E-Commerce Shipping Data** from Kaggle.

### 🚀 **Dataset Overview**
------------------------------------------------

The dataset consists of **10,999 observations** and **12 features**, including:

*   **Customer data** (ID, Gender)
*   **Product data** (Cost, Importance)
*   **Shipping data** (Warehouse Block, Mode of Shipment, Customer Care Calls, Weight)
*   **Target variable**: Whether the product reached on time (1 = No, 0 = Yes)

### 📊 **Model Performance Comparison**
------------------------------------------------

#### **Decision Tree**

*   Accuracy increased by 0.62%.
*   Precision rose from 69.76% to 85.77%, but recall dropped significantly.
*   F1-Score showed a notable decrease, signaling overfitting.

#### **Naïve Bayes**

*   No performance change after tuning. A stable model, but rigid due to independence assumptions.

#### **K-Nearest Neighbours (KNN)**

*   A slight accuracy improvement (from 54.42% to 55.67%).
*   Precision increased by 1%, while recall rose from 47.75% to 51.00%.
*   This tuning helped balance precision and recall, though KNN is still not efficient on large datasets.

#### **Random Forest**

*   Accuracy decreased from 60.63% to 60.25%, but precision improved from 73.11% to 80.07%.
*   Recall dropped after tuning, indicating a more conservative model that misses positive predictions.

#### **Support Vector Machine (SVM)**

*   Accuracy improved from 55.67% to 58.43%.
*   Precision surged from 57.25% to 75.09%, but recall decreased substantially.
*   The tuning made the model more cautious, leading to missed positive instances.

### 💡 **Model Weaknesses & Insights**
------------------------------------------------

*   **Decision Tree**: Overfitting issues are apparent, with a loss in recall after tuning. A more complex model might be needed for better generalization.
*   **Naïve Bayes**: While stable, it does not adapt well to this specific dataset's feature dependencies.
*   **KNN**: Struggles with large datasets due to its reliance on distance metrics and computational inefficiency.
*   **Random Forest**: Tuning made it more conservative, which led to fewer positive predictions.
*   **SVM**: Highly sensitive to hyperparameter tuning, affecting its ability to correctly identify positive instances.

### 🏁 **Conclusion & Future Directions**
------------------------------------------------

*   Hyperparameter tuning can boost **precision** but sometimes at the cost of **recall**.
*   Both **Random Forest** and **Decision Tree** showed strong potential, but their performance needs further tuning to balance precision and recall.
*   Future work will explore **Gradient Boosting** models (XGBoost, LightGBM, CatBoost) for potentially better performance with regularization to handle overfitting.

### 📈 **Key Takeaways**
------------------------------------------------

*   Tuning models for precision can result in sacrificing recall, making it essential to balance both based on the business need.
*   **Random Forest** and **Decision Tree** are solid starting points, but **Gradient Boosting** could offer better overall performance.
*   The project demonstrates the complexity of e-commerce logistics, where predictive accuracy can directly impact operational efficiency.
