# Car Price Prediction Using Machine Learning

## 1. Project Overview

This project focuses on predicting car prices using Machine Learning regression algorithms.

A Chinese automobile company plans to enter the US market and wants to understand the factors that influence car prices. This project uses automobile data from the American market to identify the important factors affecting car prices and build predictive models.

The project applies different regression algorithms, compares their performance, identifies the best-performing model, and performs hyperparameter tuning to improve prediction accuracy.

## 2. Business Objective

The main objectives of this project are:

- To identify the important variables that influence car prices.
- To understand how different automobile features affect pricing.
- To build Machine Learning models to predict car prices.
- To compare different regression algorithms and identify the best-performing model.
- To improve model performance through hyperparameter tuning.

## 3. Dataset Description

The dataset contains information about different automobiles in the American market.

**Dataset Source:** [Car Price Prediction Dataset](https://drive.google.com/file/d/1FHmYNLs9v0Enc-UExEMpitOFGsWvB2dP/view?usp=drive_link)

**Target Variable:** `price`

The target variable represents the price of a car. The remaining relevant columns are used as independent variables to predict the price.

## 4. Technologies and Libraries Used

- Python
- Jupyter Notebook
- Pandas – Data loading and manipulation
- NumPy – Numerical operations
- Matplotlib – Data visualization
- Seaborn – Statistical visualization
- Scikit-learn – Machine Learning models, preprocessing, evaluation and hyperparameter tuning

## 5. Project Workflow

### Step 1: Data Loading and Preprocessing

- Loaded the automobile dataset using Pandas.
- Examined the dataset structure, columns and data types.
- Checked for missing values and duplicate records.
- Performed necessary data cleaning and preprocessing.
- Separated independent variables (X) and the target variable (y).
- Applied suitable preprocessing techniques to numerical and categorical features.
- Split the dataset into training and testing sets.

### Step 2: Exploratory Data Analysis (EDA)

Performed exploratory data analysis using visualizations to understand the dataset and relationships between different automobile features and car prices.

Visualizations included:
- Price distribution histogram.
- Boxplot for identifying outliers.
- Correlation heatmap.
- Engine size versus price scatter plot.

### Step 3: Model Implementation

Implemented and trained the following five regression algorithms:

1. Linear Regression
2. Decision Tree Regressor
3. Random Forest Regressor
4. Gradient Boosting Regressor
5. Support Vector Regressor (SVR)

### Step 4: Model Evaluation

Evaluated and compared the models using the following performance metrics:

- **R² Score:** Measures how well the model explains the variation in car prices. A higher value indicates better performance.
- **Mean Squared Error (MSE):** Measures the average squared difference between actual and predicted prices. A lower value is better.
- **Mean Absolute Error (MAE):** Measures the average absolute difference between actual and predicted prices. A lower value is better.

The best-performing model was selected based on the comparison of these evaluation metrics.

### Step 5: Feature Importance Analysis

Performed feature importance analysis to identify the significant variables influencing car prices.

This analysis helps understand which automobile features contribute more to price prediction.

### Step 6: Hyperparameter Tuning

Applied hyperparameter tuning using GridSearchCV to identify suitable model parameters and improve the performance of the selected model.

The performance was compared before and after tuning using R² Score, MSE and MAE.

## 6. Final Model Results

After model comparison and hyperparameter tuning, the **Random Forest Regressor** was identified as the tuned model.

### Tuned Random Forest Performance

| Evaluation Metric | Result |
|---|---:|
| R² Score | 0.9595 |
| MSE | 3,195,239.52 |
| MAE | 1,251.49 |

### Interpretation

- The R² score of 0.9595 indicates that the model explains approximately 95.95% of the variation in car prices in the test dataset.
- The MSE measures the squared prediction errors.
- The MAE indicates that the model's predictions differ from actual car prices by approximately 1,251.49 price units on average.

Hyperparameter tuning improved the model's performance by increasing the R² score and reducing both MSE and MAE.

## 7. Conclusion

This project demonstrates how Machine Learning regression algorithms can be used to predict automobile prices based on different car features.

Five regression models were implemented and evaluated using R² Score, MSE and MAE. Feature importance analysis was also performed to identify significant variables affecting car prices.

The tuned Random Forest Regressor achieved an R² score of 0.9595, demonstrating strong predictive performance on the test dataset.

Overall, this project helps understand automobile pricing factors and demonstrates the application of Machine Learning techniques in solving a real-world regression problem.

## 8. Repository Contents

- `Codeathon.ipynb` – Jupyter Notebook containing the Python code, preprocessing, visualizations, model implementation, evaluation, feature importance analysis and hyperparameter tuning.
- `README.md` – Project documentation.
- `CarPrice_Assignment.csv` – Dataset file (if included in the repository).

## 9. How to Run the Project

1. Clone or download this repository.
2. Install the required Python libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```

3. Open the Jupyter Notebook.
4. Ensure the dataset is available in the correct location.
5. Run the notebook cells sequentially to perform the analysis and model training.

---

**Project Title:** Car Price Prediction Using Machine Learning  
**Project Type:** Machine Learning – Regression  
**Target Variable:** `price`
