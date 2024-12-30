# Phishing-website-detection-using-machine-learning

The project aims to build and evaluate machine learning models that can effectively classify websites as phishing or legitimate based on their features. The use of data balancing, visualization, and various models demonstrates a comprehensive approach to tackling the phishing detection problem.

---

## Data Loading and Exploration
1. **Dataset Loading**: The project begins by loading the `phishing.csv` dataset.
2. **Exploratory Analysis**:
   - Used functions like `head()`, `info()`, and `isnull().sum()` to understand the data structure and check for missing values.

---

## Data Balancing
- The target variable (`class`), which indicates whether a website is phishing or legitimate, was found to be imbalanced.
- To address this, the `RandomOverSampler` technique was employed, ensuring equal representation of both classes for better model training.

---

## Data Visualization
Several visualizations were created to gain insights into the data:

1. **Bar Plots**:
   - Distribution of the target variable before and after balancing.
   - Comparison of counts for `LongURL` and `ShortURL` features.

2. **Feature Importance**:
   - Used `ExtraTreesClassifier` to visualize the most influential features.

3. **Feature Relationships**:
   - Explored the relationship between `AnchorURL` and `HTTPS` using a stacked bar chart.

4. **Correlation Heatmap**:
   - Displayed relationships between different features to identify patterns.

---

## Model Training and Evaluation
Various machine learning models were trained to detect phishing websites:

- **Random Forest**
- **Decision Tree**
- **SVM (Support Vector Machine)**
- **Naive Bayes**
- **Gradient Boosting**
- **LightGBM**
- **CatBoost**

### Evaluation Metrics:
- Accuracy scores and classification reports were generated for each model to assess their performance.

---

## Model Comparison
- A bar plot was used to compare the accuracies of different models.
- This helped identify the best-performing model(s).

---

## Hybrid Model Exploration
- The project explored hybrid models by combining different base models using `VotingClassifier`.
- The accuracies of these hybrid models were compared to assess improvements in performance.

---
Thank you 😊
