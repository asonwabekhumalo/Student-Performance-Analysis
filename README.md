# Student-Performance-Prediction
Machine learning project predicting student performance using Python and scikit-learn.
<p align="center">
  <img src="Student Performance Cover Page.png" alt="Student Performance Prediction Cover" width="100%">
</p>

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
    <td>K-Nearest Neighbors</td>
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
The K-Nearest Neighbors Regressor was chosen as it achieved the best performance with an MAE of 5.066, an RMSE of 6.367, and an R² score of -0.5. However, needed to be tuned due to the negative R². 


## KNN Hyperparameter Tuning
The K-Nearest Neighbours model was tuned by varying the number of neighbours (k).
Different values of n_neighbors were tested and compared using validation MAE, RMSE, and R².

80 neighbors were chosen for the final KNN model as it provided the best validation performance.


## Model Evaluation
For the tuned KNN model, the test-set R² of 0.141 indicates that approximately 14.1% of the variation in final grades was explained by the model.


## Key Findings
The analysis found that:
<li>Previous academic performance was strongly associated with final grades.
<li>Second-period grades had the strongest positive correlation with final grades.
<li>First-period grades also showed a strong positive relationship with final grade.
<li>Failures was the strongest negative correlation with final grades
<li>Other academic, demographic, and lifestyle variables generally showed weaker linear associations.
<li>Model performance varied across the different regression algorithms.


## Technologies Used:
<li>Python
<li>Pandas
<li>NumPy
<li>Matplotlib
<li>Seaborn
<li>Scikit-learn
<li>Jupyter Notebook


## Recommendations
<li><strong>Early detection:</strong><li> Schools could use students' earlier assessment grades to identify students who may be at risk of poor final performance, allowing teachers to intervene earlier and provide additional academic support.
<li><strong>Targeted academic support:</strong> Students showing signs of academic difficulty could receive additional support, such as tutoring and extra classes, before the final assessment.
<li><strong>Expand the dataset:</strong> Future studies could use larger datasets and include additional variables, such as student attendance and assessments of sleep and eating habits, to provide a more comprehensive understanding of the factors associated with academic performance.
<li><strong>Improve generalisability:</strong> The models should be tested using students from different schools, regions, and educational systems before being applied in practice, as the current dataset represents students from specific Portuguese schools.

  
## 📁Project Structure
Student-Performance-Prediction/
│
├── student_data.csv
├── Student_Performance_Prediction.ipynb
└──README.md


## References
UCI Machine Learning Repository — Student Performance Dataset
Scikit-learn documentation

