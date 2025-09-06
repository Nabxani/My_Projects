# **Overview**



This project analyzes English football player injury data and predicts days and games missed as well as classifies injuries by severity. The analysis demonstrates a full data science workflow including EDA, regression, classification, handling class imbalance, and visualization.



### **Dataset**



**Source:** Kaggle Football Datasets



**File used:** player\_injuries.csv



###### **Key columns:**



player\_id – unique player identifier



season\_name – football season



injury\_reason – type of injury



from\_date, end\_date – injury period



days\_missed – total days absent



games\_missed – total matches missed



#### 

#### **Steps in the Notebook**



###### **1. Data Cleaning**



* Converted date columns to datetime
* Filled missing days\_missed using date differences
* Dropped rows with critical missing values





###### **2. Exploratory Data Analysis (EDA)**





* Injuries per season – bar plot showing trends



* Top injury reasons – most common types of injuries



* Players with most injuries – identifies high-risk players



* Distribution plots – visualize days missed and games missed



* Scatter plots – relationship between days missed and games missed





###### **3. Regression Models**





Predicted days\_missed and games\_missed using Random Forest Regressor





**Evaluation metrics:**



* Days Missed → RMSE ~50, R² ~0.40



* Games Missed → RMSE ~7, R² ~0.32



* Scatter plots of actual vs predicted values



###### 

###### **4. Classification Models**





Multi-class classification: Short / Medium / Long-Term injuries



* Short-Term: ≤30 days



* Medium-Term: 31–90 days



* Long-Term: >90 days



Used SMOTE to handle class imbalance



Random Forest Classifier with class\_weight='balanced'





###### **Evaluation:**



Overall accuracy: ~60%



F1-score highest for Short-Term injuries (~0.73)



Long-Term recall improved (~0.58)





###### **Visualizations:**



Confusion matrix heatmap



Feature importance

