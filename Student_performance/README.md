# Student Performance Analysis



This project analyzes a student performance dataset to explore how demographic and preparation factors affect exam results. The analysis is implemented in a Jupyter/Colab notebook and includes both regression and classification tasks.



## 📊 Dataset



### Columns:



gender



race/ethnicity



parental level of education



lunch



test preparation course



math score



reading score



writing score



## 🎯 Tasks



Regression → Predict a student’s Math Score from demographics and other scores.



Classification → Predict whether a student passes Math (≥ 60 = pass, < 60 = fail).



## 🔍 Methods



Exploratory Data Analysis (EDA): distributions, correlations, group comparisons



Feature Engineering: creation of pass/fail target



Preprocessing: scaling numeric features, one-hot encoding categorical features



### Models:



Regression → Random Forest Regressor



Classification → Random Forest Classifier



### Evaluation Metrics:



Regression → RMSE, MAE, R²



Classification → Accuracy, Precision, Recall, F1-score, Confusion Matrix



## 📈 Results



Math, reading, and writing scores are strongly correlated



Lunch type and test preparation course significantly affect performance



Random Forest models achieved strong predictive performance in both regression and classification tasks

