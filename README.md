## Title:
## 🔹 Polycystic Ovary Syndrome (PCOS) Prediction Project

## 📌 Project Description:
### Dataset Used
I chose the "PCOS Dataset" from Kaggle, which contains anonymized clinical and diagnostic data for women, including whether or not they were diagnosed with PCOS. The dataset involves a classification task, where the goal is to predict the presence of PCOS based on various medical and physical indicators.

### Why This Project?
Polycystic Ovary Syndrome (PCOS) is a common but underdiagnosed condition that affects hormonal levels in women. Early prediction can help in timely treatment and lifestyle adjustments. I found this problem compelling due to its real-world impact in healthcare and the opportunity to work with clinical features — a practical domain for machine learning applications.

## Steps Taken
### 1. Data Preprocessing
- No missing values were found in the dataset — all features were complete, so no imputation or row removal was needed.

- Standardized continuous variables like BMI and hormone levels using StandardScaler to ensure consistent feature scaling.

- All features were numerical, so no encoding was necessary.

### 2. Feature Engineering
Since BMI was already present and no derived features were strictly necessary, I focused on:

- Checking for multicollinearity using a correlation heatmap

- Verifying the distribution of features by class using boxplots and histograms.

### 3. Data Visualization
To better understand the relationships:

- Created a Heatmap of correlation matrix to identify highly correlated features.
The heatmap suggests that Menstrual Irregularity and BMI are relatively important factors in PCOS diagnosis, while Age may have a minor influence.

- Box plot comparing testosterone levels in patients with and without Polycystic Ovary Syndrome (PCOS). 

- Histograms for BMI, Age distribution across classes.

- Scatter plot illustrating the relationship between testosterone levels and antral follicle count in individuals. 
The Scatter plot indicates that individuals with PCOS tend to have a higher antral follicle count, but there's no clear correlation between testosterone levels and antral follicle count.

- A bar graph that illustrates the relationship between menstrual irregularity and PCOS (Polycystic Ovary Syndrome) diagnosis. indicating that individuals with irregular menstrual cycles are more likely to be diagnosed with PCOS.

These visualizations helped identify key contributing factors to PCOS (e.g., high AMH and BMI).

### 4. Model Selection
Given it’s a binary classification task, I compared a few models:

Logistic Regression

Random Forest

XGBoost

Support Vector Machine (SVM)

I chose Random Forest as my primary model because:

It handles feature interactions and non-linearities well.

It provides feature importance which aids interpretability.


### 5. Model Evaluation
Used an 80/20 train-test split.

Model Used: Random Forest Classifier

Accuracy: 99.0%


## Challenges & Solutions
The dataset was clean and complete, requiring no imputation or row removal.

## Conclusion
The PCOS prediction model shows promising performance and could be used as a supportive diagnostic tool. This project taught me a lot about handling real-world medical data, feature engineering in the health domain, and balancing precision vs recall in critical applications.

