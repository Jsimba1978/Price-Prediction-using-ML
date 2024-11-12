# Price-Prediction-using-ML

This project builds a machine learning model to predict house prices based on various features such as property characteristics and location details. The model leverages several regression techniques to deliver accurate price predictions, making it a valuable tool for real estate analysis.

## Dataset

The dataset used for this project includes 13 features that provide information about different aspects of houses:

1. **Id** - Unique identifier for each record.
2. **MSSubClass** - Type of dwelling.
3. **MSZoning** - General zoning classification.
4. **LotArea** - Lot size in square feet.
5. **LotConfig** - Configuration of the lot.
6. **BldgType** - Type of dwelling.
7. **OverallCond** - Overall condition rating of the house.
8. **YearBuilt** - Year when the house was originally constructed.
9. **YearRemodAdd** - Year of remodeling or addition.
10. **Exterior1st** - Exterior covering type.
11. **BsmtFinSF2** - Secondary finished square feet of basement.
12. **TotalBsmtSF** - Total square feet of basement area.
13. **SalePrice** - Sale price of the house, which serves as the target variable.

## Project Workflow

1. **Data Preprocessing**:
   - Identify data types (categorical, integer, float).
   - Handle missing values and remove irrelevant columns to ensure data consistency.

2. **Exploratory Data Analysis (EDA)**:
   - Use heatmaps and barplots to visualize relationships and correlations in the dataset.

3. **Data Cleaning**:
   - Drop irrelevant columns, fill missing values, and use encoding techniques (e.g., OneHotEncoding) to prepare categorical features.

4. **Model Training**:
   - Train multiple regression models:
     - Support Vector Machine (SVM)
     - Random Forest Regressor
     - Linear Regression
     - CatBoost Regressor

5. **Model Evaluation**:
   - Evaluate models using metrics like Mean Absolute Percentage Error (MAPE) and R-squared to select the most accurate model.

## Key Libraries

This project uses the following Python libraries:
- **Pandas** for data manipulation.
- **Matplotlib** and **Seaborn** for data visualization.
- **scikit-learn** for implementing machine learning models.
- **CatBoost** for gradient boosting models.

## Model Comparison

| Model                 | Mean Absolute Percentage Error (MAPE) |
|-----------------------|---------------------------------------|
| Support Vector Machine| 0.18                                  |
| Random Forest         | 0.19                                  |
| Linear Regression     | 0.18                                  |
| CatBoost              | 0.11                                  |

## Conclusion

Among all models tested, the **CatBoost Regressor** delivered the best performance with an R² score of 0.89, making it the most accurate model for this project. Future improvements could involve applying ensemble techniques like Bagging and Boosting to potentially enhance the model’s predictive power.

