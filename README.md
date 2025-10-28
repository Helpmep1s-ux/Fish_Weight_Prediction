# Fish Weight Prediction

In this repository, **Linear Regression** is used to predict the weight of fish based on their features. The dataset from [Fish Market dataset](https://www.kaggle.com/datasets/aungpyaeap/fish-market) is used, the model predicts fish weight using features such as length, height, width, and species.

## Dataset Overview

The dataset has 159 rows and 7 columns:

- **Species**: Type of fish (e.g., Bream, Perch)
- **Weight**: Weight of the fish in grams (target variable)
- **Length1**: Vertical length in cm
- **Length2**: Diagonal length in cm
- **Length3**: Cross length in cm
- **Height**: Height in cm
- **Width**: Width in cm

## Methodology

 A **Linear-Regression** model is used to predict the weight of the fish. The steps involved are:

1. **Data Preprocessing**:
   * Data Wrangling was done to change all data to integer, float or bool type.
   * After data wrangling, Exploratory Data Analysis (EDA) is done to understand about data distrubution and relationship between features.
   * For EDA matplotlib and seaborn library were used to visualize the data. The skewness of data was observed. Then correlation between features were seen. Outliers were handled using Inter-Quartile Range (IQR).
   * Finally train.csv was created.
2. **Model Training**:
    * Linear Regression model was trained by splitting the data into train(0.6), validation(0.2) and test(0.2).
    * Model from scikit-learn was also used.
3. **Model Evaluation**: 
    * The mse loss, rmse loss, r2-score were used to evaluate the model.

## Project Structure

- **Dataset/**: Contains the raw dataset.
- **notebooks/**: Jupyter notebooks for data wrangling, exploratory data analysis, model training, and evaluation.
- **requirements.txt**: Lists the necessary Python packages.
