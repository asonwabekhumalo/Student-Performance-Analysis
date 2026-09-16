# Student-Performance-Prediction
Machine learning project predicting student performance using Python and scikit-learn.

## Project Overview
This project analyses a student performance dataset and develops machine learning regression models to predict students' final grades. The project follows a complete data science workflow, including data exploration, data cleaning, feature preparation, model training, and model evaluation.

## Dataset
The data used for this project is the <strong>UCI Student Performance dataset</strong>, which contains information about students' academic performance, demographic characteristics, family background, and lifestyle factors. It was obtained from <strong>Kaggle</strong>, a widely recognized platform for publicly available datasets for data science and machine learning projects.

The dataset contains <strong>395 records</strong> and <strong>33 features</strong> which includes both categorical and numerical variables such as age, gender, family size and parents' occupations. The 33 features include a <strong>target ("G3")</strong> which indicates the final grade that the student achieved. 

This dataset was chosen because it contains a mixture of categorical and numerical features, which allows for implementation preprocessing techniques such as encoding and normalization. These characteristics then make the dataset ideal for demonstrating knowledge in <strong>data preprocessing, exploratory data analysis, feature engineering, and machine learning model development</strong>.

## Objectives:
<li>Perform exploratory data analysis.
<li>Explore the factors that influence student performance.
<li>Prepare the dataset for machine learning.
<li>Build regression models to predict students' final grades.
<li>Compare the performance of different regression algorithms.
<li>Evaluate the chosen algorithms performance.


## Exploratory Data Analysis
Exploratory data analysis was conducted to understand the dataset and identify patterns associated with students' final grades.

<li>The analysis included:
<li>Data quality checks
<li>Descriptive statistics
<li>Distribution analysis
<li>Correlation analysis
<li>Boxplots
<li>Analysis of academic performance trends

The correlation analysis showed that previous academic performance had the strongest relationship with final grades, particularly the first-period (G1) and second-period (G2) grades.

## Data Preprocessing
<li>The following preprocessing steps were performed:
<li>Checked for missing values
<li>Checked for duplicate records
<li>Add a column student_id uniquely identify each student for for the spaghetti plot
<li>Removed the student_id identifier
<li>Encoded categorical variables
<li>Prepared the features and target variable
<li>Scaled features where required by the machine learning model
<li>Split the data into training, validation, and test sets

A 60% training, 20% validation, and 20% test split was used.


## Machine Learning Models
Four regression models were developed:
**1.** Linear Regression
**2.** Neural Network Regression
**3.** K-Nearest Neighbours (KNN) Regression
**4.** Random Forest Regression

The models were evaluated using:
<li>Mean Absolute Error (MAE)
<li>Root Mean Squared Error (RMSE)
<li>R² (R-squared)

## Model Comparison
The validation set was used to compare the models, while the test set was reserved for the final evaluation of the selected model.
<table>
  <tr>
    <th>Model</th>
    <th>MAE</th>
    <th>RMSE</th>
    <th>R²</th>
  </tr>
  <tr>
    <td>Linear Regression</td>
    <td>206.064</td>
    <td>222.623</td>
    <td>-2047.9</td>
  </tr>
  <tr>
    <td>Neural Network</td>
    <td>76.449</td>
    <td>79.555</td>
    <td>-206.648</td>
  </tr>
  <tr>
    <td>K-Nearest Neighbours</td>
    <td>5.066</td>
    <td>6.367</td>
    <td>-0.676</td>
  </tr>
  <tr>
    <td>Random Forest</td>
    <td>7.812</td>
    <td>9.039</td>
    <td>-2.378</td>
  </tr>
</table>
