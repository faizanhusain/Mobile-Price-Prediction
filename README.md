# Mobile-Price-Prediction
The purpose of this project is to build a system capable of predicting mobile phone pricing categories (low, medium, high, very high) based on market data. This involves exploring the dataset, analyzing features, and implementing predictive models to achieve this goal.

## Data Analysis and Feature Exploration
### 1) Exploratory Data Analysis (EDA)
 ### Key Findings:
 - Correlation Analysis: Features like RAM and pixel resolutions were highly correlated with price range.
 - Visualizations: Scatterplots, histograms, and heatmaps were used to visualize relationships.
   - RAM showed a clear distinction between price ranges.
   - Higher battery capacity generally correlated with higher price categories.
### 2) Feature Comparison
  ### Comparison Across Features:
  - RAM vs. Price Range:
    - Phones with higher RAM were consistently in the higher price ranges. This feature had the strongest distinction among categories.
  - Battery Power vs. Price Range
    - While higher battery power indicated a tendency towards higher price ranges, the correlation was weaker compared to RAM.
  - Pixel Resolution (Height and Width):
    - Screen resolution had a noticeable impact, with better resolutions found in higher-priced phones.
  - Camera (Primary and Front):
    - Primary camera resolution showed more significant variation across price categories than front camera resolution.
  - Features (4G, 3G, WiFi):
    - Most phones supported 3G and WiFi regardless of price range, while 4G availability was more common in higher-priced models.
### 3) Feature Engineering and Preprocessing
- Normalization and Standardization: Applied using MinMaxScaler and StandardScaler to normalize features.
- Handling Categorical Data: Binary features like Bluetooth, 4G, and 3G were retained as-is.
- Splitting Data: Divided into training and test sets using an 80-20 split.
# Model Building and Evaluation
  ### 1) Machine Learning Models
  - Random Forest Classifier
  - Gradient Boosting Classifier
  - Logistic Regression
  - XGBoost
  - Neural Networks (MLP and TensorFlow)
 ### 2)  Model Performance:
    Evaluation metrics included accuracy, precision, recall, and ROC-AUC. Cross-validation and grid/randomized search were used for hyperparameter tuning.
  - Random Forest: Achieved high accuracy (~90%) with default parameters.
  - Gradient Boosting: Performed comparably, especially after hyperparameter tuning.
  - XGBoost: Provided slightly better performance with optimized learning rates and tree depth.
  - Neural Networks: Achieved competitive results but required more computational resources.
### 3) Feature Importance
- RAM was identified as the most significant feature.
- Pixel resolution and battery capacity also contributed significantly.


# Conclusion and Recommendations
    The project successfully built a system to predict mobile price categories with high accuracy.
- RAM, pixel resolution, and battery capacity are strong predictors of mobile pricing.
- Ensemble models like Random Forest and XGBoost are highly effective for this task.
- Further improvements could involve:
  - Incorporating additional features such as brand or software.
  - Exploring deep learning architectures for enhanced performance.
