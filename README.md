# Student-Performance-Prediction
Machine learning project predicting student performance using Python and scikit-learn.

Project Overview
This project analyses a student performance dataset and develops machine learning regression models to predict students' final grades. The project follows a complete data science workflow, including data exploration, data cleaning, feature preparation, model training, and model evaluation.

Objectives:
- Explore the factors that influence student performance.
- Perform exploratory data analysis using visualisations.
- Prepare the dataset for machine learning.
- Build regression models to predict students' final grades.
- Compare the performance of different regression algorithms.


Dataset:
The dataset consists of 33 columns including the target variable final grade (G3) and 395 rows. The dataset contains information about students' demographic, social, and academic characteristics.

Example features include:
- Age
-  Study time
- Absences
- Previous grades (G1 and G2)
- Internet access
- Extracurricular activities


The following visualisations were created:
- Gender distribution
- Pass/Fail distribution 
- Grade distribution histogram
- Final Grade vs Absences
- Study Time vs Final Grade
- Internet Access vs Final Grade
- Activities vs Final Grade
- Weedday and Weeked Alcohol Consumption vs Final Grade
- Health vs Final Grade
- Final Grade vs G1
- Final Grade vs G2


Key findings:
- Students with higher G1 and G2 grades generally achieved higher final grades.
- Higher absenteeism tended to be associated with lower final grades.
- Students with internet access generally achieved slightly better grades.
- Study time showed a positive relationship with academic performance.
- Less travel time was associated with good academic performance. 
- Students with higher failures achieved lower final grades. 


The following preprocessing steps were performed:
- Checked for missing values
- Checked for duplicate records
- One-hot encoded categorical variables
-  Normalised numerical features using MinMaxScaler
- Split the data into training and testing sets (80/20)


Models Used:
- Linear Regression
- Neural Network Regressor 
- K-Nearest Neighbours Regressor 
- Decision Tree Regressor


The models were evaluated using:
- Mean Absolute Error 
- Mean Squared Error 
- Root Mean Squared Error 
- R-square Score

Key Findings:
The Decision Tree Regressor achieved the best performance with an MAE of 0.88, an RMSE of 1.323, and an R² score of 0.924.


Technologies Used:
- Python
- pandas
- NumPy
- Matplotlib
- scikit-learn
- Seaborn
- Jupyter Notebook



